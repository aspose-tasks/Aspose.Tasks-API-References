---
title: "PageInfo.PageInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PageInfo. Инициализирует новый экземпляр класса PageInfo. Представляет данные настройки страницы, которые присутствуют в формате файла MPP и используются для печати"
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/pageinfo/pageinfo/
---
## PageInfo constructor

Инициализирует новый экземпляр класса [`PageInfo`](../). Представляет данные настройки страницы, которые присутствуют в формате файла MPP и используются для печати.

```csharp
public PageInfo()
```

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

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


