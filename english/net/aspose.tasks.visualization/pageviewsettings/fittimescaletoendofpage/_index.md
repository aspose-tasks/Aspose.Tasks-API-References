---
title: PageViewSettings.FitTimescaleToEndOfPage
second_title: Aspose.Tasks for .NET API Reference
description: PageViewSettings property. Gets or sets a value indicating whether to fit timescale to the end of a page when printing
type: docs
weight: 30
url: /net/aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/
---
## PageViewSettings.FitTimescaleToEndOfPage property

Gets or sets a value indicating whether to fit timescale to the end of a page when printing.

```csharp
public bool FitTimescaleToEndOfPage { get; set; }
```

## Examples

Shows how to print task, resource, assignment notes on a separate page.

```csharp
var project = new Project(DataDir + "Input.mpp");

// set the number of first columns to be printed on all pages
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// set a value indicating whether to print notes.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// set a value indicating whether to fit timescale to the end of a page when printing.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// set a value indicating whether to print all sheet columns of a view
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// set a value indicating whether to print blank pages of a view
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// set a value indicating whether to print a specified number of first columns on all pages
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


