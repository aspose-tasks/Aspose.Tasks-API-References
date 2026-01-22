---
title: Class PageViewSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageViewSettings class. Represents printing settings for a project view
type: docs
weight: 3230
url: /net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Represents printing settings for a project view.

```csharp
public class PageViewSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Gets or sets the number of first columns to be printed on all pages. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Gets or sets a value indicating whether to fit timescale to the end of a page when printing. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Gets or sets a value indicating whether to print all sheet columns of a view. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Gets or sets a value indicating whether to print blank pages of a view. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Gets or sets a value indicating whether to print a specified number of first columns on all pages. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Gets or sets a value indicating whether to print notes. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


