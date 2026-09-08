---
title: "Класс TableTextStyle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.TableTextStyle. Представляет стиль текста в таблице представления."
type: docs
weight: 3370
url: /ru/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Представляет стиль текста в таблице представления.

```csharp
public class TableTextStyle : TextStyle
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Инициализирует новый экземпляр класса `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Инициализирует новый экземпляр класса `TableTextStyle` с указанным шрифтом. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Инициализирует новый экземпляр класса `TableTextStyle` с настройками шрифта по умолчанию и указанным стилем шрифта. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Инициализирует новый экземпляр класса `TableTextStyle` с указанным размером шрифта и стилем шрифта. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Получает или задает цвет фона стиля текста. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Получает или задает шаблон фона стиля текста. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Получает или задает цвет текста. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Получает или задает поле, к которому применяется стиль. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Получает или задает шрифт стиля текста. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Возвращает значение перечисления [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Получает уникальный идентификатор строки. Возвращает -1, если стиль применяется ко всем строкам представления. |

## Примеры

Показывает, как настраивать стили текста таблицы, которые используются для оформления различных текстовых элементов в проекте.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// установить стиль текста первого названия задачи
var style1 = new TableTextStyle(1);
// установить поле, к которому будет применён стиль.
style1.Field = Field.TaskName;
// установить <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> стиля текста.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// установить размер шрифта стиля текста в пунктах.

// установить стиль текста второй продолжительности задачи
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // установить флаг, указывающий, что данные представления должны быть записаны
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### См. также

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


