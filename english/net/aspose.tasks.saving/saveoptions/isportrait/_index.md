---
title: SaveOptions.IsPortrait
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether the page orientation is portrait returns false if the page orientation is landscape
type: docs
weight: 70
url: /net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

```csharp
public bool IsPortrait { get; set; }
```

## Remarks

Is not applicable when SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In this case View.PageInfo.PageSettings.IsPortrait is used instead. Is not applicable when SaveOptions.CustomPageSize is set.

## Examples

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


