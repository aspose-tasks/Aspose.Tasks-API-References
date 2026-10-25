---
title: "Класс TextStyle"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.TextStyle. Измените визуальный стиль текста для элемента в представлении проекта"
type: docs
weight: 3420
url: /ru/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Изменить визуальный стиль текста для элемента в представлении проекта.

```csharp
public class TextStyle
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Инициализирует новый экземпляр класса `TextStyle` с настройками по умолчанию. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Инициализирует новый экземпляр класса `TextStyle` с указанными параметрами шрифта. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Инициализирует новый экземпляр класса `TextStyle` с шрифтом по умолчанию и указанным стилем шрифта. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Инициализирует новый экземпляр класса `TextStyle` с шрифтом по умолчанию и указанными размером и стилем шрифта. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Получает или задает цвет фона стиля текста. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Получает или задает шаблон фона стиля текста. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Получает или задает цвет текста. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Получает или задает шрифт стиля текста. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Получает или задает [`TextItemType`](../textitemtype/) стиля текста. |

## Примеры

Показывает, как настраивать стили текста, которые используются для оформления различных текстовых элементов в проекте.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


