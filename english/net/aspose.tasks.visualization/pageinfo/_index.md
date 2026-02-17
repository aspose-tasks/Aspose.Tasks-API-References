---
title: Class PageInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageInfo class. Represents page setup data which is present in MPP file format and used for printing
type: docs
weight: 3180
url: /net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

Represents page setup data which is present in MPP file format and used for printing.

```csharp
public class PageInfo
```

## Constructors

| Name | Description |
| --- | --- |
| [PageInfo](pageinfo/)() | Initializes a new instance of the `PageInfo` class. Represents page setup data which is present in MPP file format and used for printing. |

## Properties

| Name | Description |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | Gets or sets an instance of the [`HeaderFooterInfo`](../headerfooterinfo/) class which represents a footer data. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | Gets or sets the instance of the [`HeaderFooterInfo`](../headerfooterinfo/) class which represents a header data. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | Gets or sets an instance of the [`PageLegend`](../pagelegend/) class which specifies rendering options of page legend. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | Gets an instance of the [`PageMargins`](../pagemargins/) class which specifies page margins. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | Gets the name of the view for which set-up data is used. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | Gets an instance of the [`PageSettings`](./pagesettings/) class which specifies page printing settings. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | Gets an instance of the [`PageViewSettings`](./pageviewsettings/) class which specifies page view printing settings. |

## Examples

Shows how to work with page info of MS Project view.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// lets modify the default view
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// lets modify margins
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// lets modify page settings
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// lets modify page view settings
// set a value indicating whether to print notes.
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

// work with project...
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


