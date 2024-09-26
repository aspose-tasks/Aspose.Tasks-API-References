---
title: PageInfo.PageViewSettings
second_title: Aspose.Tasks for .NET API Reference
description: PageInfo property. Gets an instance of the PageViewSettings class which specifies page view printing settings
type: docs
weight: 80
url: /net/aspose.tasks.visualization/pageinfo/pageviewsettings/
---
## PageInfo.PageViewSettings property

Gets an instance of the `PageViewSettings` class which specifies page view printing settings.

```csharp
public PageViewSettings PageViewSettings { get; }
```

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

* class [PageViewSettings](../../pageviewsettings/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


