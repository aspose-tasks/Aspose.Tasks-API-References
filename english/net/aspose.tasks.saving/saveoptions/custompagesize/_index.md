---
title: SaveOptions.CustomPageSize
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the custom page size in points 1 point  1/72 of inch
type: docs
weight: 20
url: /net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Gets or sets the custom page size in points (1 point = 1/72 of inch).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Examples

Shows how to set custom page size when project is saved to PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


