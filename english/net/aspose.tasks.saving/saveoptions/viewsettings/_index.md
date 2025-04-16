---
title: SaveOptions.ViewSettings
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a view View to render. You can use this options to explicitly specify which view should be saved to PDF HTML or Image formats. If this property is set PresentationFormat property is ignored when project is saved. View should be from one of the following screen Screen Gantt TaskSheet TaskUsage ResourceSheet ResourceUsage
type: docs
weight: 230
url: /net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Gets or sets a view ([`View`](../view/)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) property is ignored when project is saved. View should be from one of the following screen (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

```csharp
public View ViewSettings { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | When set method is called and instance of View class with not supported value of Screen property is provided. |

## Examples

Shows how to use 'SaveOptions.ViewSettings' to specify view that should be rendered to PDf.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### See Also

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


