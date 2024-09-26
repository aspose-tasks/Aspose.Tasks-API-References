---
title: PageSettings.IsPortrait
second_title: Aspose.Tasks for .NET API Reference
description: PageSettings property. Gets or sets a value indicating whether the page orientation is portrait returns false if the page orientation is landscape
type: docs
weight: 40
url: /net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

```csharp
public bool IsPortrait { get; set; }
```

## Remarks

Is applicable during rendering when SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

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

Shows how to specify the page size and orientation using View settings or using SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// In this case the page size and orientation applied from view.PageInfo.PageSettings.PaperSize and view.PageInfo.PageSettings.IsPortrait properties.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// In this case the page size and orientation applied from properties of SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// In this case the page size applied from SaveOptions.CustomPageSize. IsPortrait property is not taken into account.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### See Also

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


