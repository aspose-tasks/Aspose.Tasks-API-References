---
title: "TableTextStyle.TableTextStyle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор TableTextStyle. Инициализирует новый экземпляр класса TableTextStyle."
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Инициализирует новый экземпляр класса [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowUid | Int32 | Указанный уникальный идентификатор строки. |

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Инициализирует новый экземпляр класса [`TableTextStyle`](../) с указанным шрифтом.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowUid | Int32 | Указанный уникальный идентификатор строки. |
| font | FontDescriptor | Шрифт, на основе которого построен текстовый стиль. |

### См. также

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Инициализирует новый экземпляр класса [`TableTextStyle`](../) с указанным размером шрифта и стилем шрифта.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowUid | Int32 | Указанный уникальный идентификатор строки. |
| fontSize | Single | Размер шрифта, на основе которого построен текстовый стиль. |
| fontStyle | FontStyles | Стиль шрифта, на основе которого построен текстовый стиль. |

### См. также

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Инициализирует новый экземпляр класса [`TableTextStyle`](../) с настройками шрифта по умолчанию и указанным стилем шрифта.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowUid | Int32 | Указанный уникальный идентификатор строки. |
| fontStyle | FontStyles | Стиль шрифта, на основе которого построен текстовый стиль. |

### См. также

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


