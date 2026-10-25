---
title: "Класс PageInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.PageInfo. Представляет данные настройки страницы, которые присутствуют в формате файла MPP и используются для печати"
type: docs
weight: 3200
url: /ru/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Представляет данные настройки страницы, присутствующие в формате файла MPP и используемые для печати.

```csharp
public class PageInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageInfo](pageinfo/)() | Инициализирует новый экземпляр класса `PageInfo`. Представляет данные настройки страницы, которые присутствуют в формате файла MPP и используются для печати. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Получает или задает экземпляр класса [`HeaderFooterInfo`](../headerfooterinfo/), который представляет данные нижнего колонтитула. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Получает или задает экземпляр класса [`HeaderFooterInfo`](../headerfooterinfo/), который представляет данные верхнего колонтитула. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Получает или задает экземпляр класса [`PageLegend`](../pagelegend/), который определяет параметры отображения легенды страницы. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Получает экземпляр класса [`PageMargins`](../pagemargins/), который определяет поля страницы. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Получает имя представления, для которого используются данные настройки. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Получает экземпляр класса [`PageSettings`](./pagesettings/), который определяет параметры печати страницы. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Получает экземпляр класса [`PageViewSettings`](./pageviewsettings/), который определяет параметры печати представления страницы. |

## Примеры

Показывает, как работать с информацией о странице в представлении MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// позволяет изменить представление по умолчанию
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// позволяет изменить поля
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// давайте изменим настройки страницы
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// давайте изменим настройки представления страницы
// установите значение, указывающее, следует ли печатать заметки.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// работать с проектом...
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


