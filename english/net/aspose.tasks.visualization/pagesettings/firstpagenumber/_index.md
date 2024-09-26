---
title: PageSettings.FirstPageNumber
second_title: Aspose.Tasks for .NET API Reference
description: PageSettings property. Gets or sets a first page number for printing
type: docs
weight: 30
url: /net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

Gets or sets a first page number for printing.

```csharp
public short FirstPageNumber { get; set; }
```

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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


