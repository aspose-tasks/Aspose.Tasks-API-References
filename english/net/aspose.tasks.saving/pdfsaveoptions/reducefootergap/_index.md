---
title: PdfSaveOptions.ReduceFooterGap
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets a value indicating whether a gap between last task and the footer must be reduced
type: docs
weight: 80
url: /net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Gets or sets a value indicating whether a gap between last task and the footer must be reduced.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Examples

Shows how to set a value indicating whether a gap between last task and the footer must be reduced in PDF output files.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


