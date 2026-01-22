---
title: Class PageSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageSettings class. Represents printing settings for a page of project view
type: docs
weight: 3210
url: /net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

Represents printing settings for a page of project view.

```csharp
public class PageSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [PageSettings](pagesettings/)() | Initializes a new instance of the `PageSettings` class. Represents printing settings for a page of project view. |

## Properties

| Name | Description |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | Gets or sets a value indicating whether to adjust printing to the specified percentage ([`PercentOfNormalSize`](./percentofnormalsize/)) of normal size. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | Gets or sets a first page number for printing. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | Gets or sets a number of pages in height to be printed. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | Gets or sets a number of pages in width to be printed. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | Gets or sets a paper size. Can be one of the values of the [`PrinterPaperSize`](../printerpapersize/) enumeration. |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | Gets or sets an integer representing one of the PrinterPaperSize values or a custom page size id. This value can be used to get PaperSize from OS settings . |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | Gets or sets a percentage of normal size to adjust printing to. |

## Examples

Shows how to work with &lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// get the settings
var settings = project.DefaultView.PageInfo.PageSettings;
// lets tune some properties
// set a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.
settings.IsPortrait = true;
// set a number of pages in width to be printed.
settings.PagesInWidth = 5;
// set a number of pages in height to be printed.
settings.PagesInHeight = 7;
// set a percentage of normal size to adjust printing to.
settings.PercentOfNormalSize = 200;
// set a paper size. Can be one of the values of the <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" /> enumeration.
settings.PaperSize = PrinterPaperSize.PaperB4;
// set a first page number for printing.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


