---
title: PrimaveraXmlSaveOptions.SkipSummaryAssignments
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraXmlSaveOptions property. Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export
type: docs
weight: 30
url: /net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Remarks

Primavera software doesn't support assignments of resources to summary (WBS) tasks. Thus, export of such assignments can result in an invalid file according to Primavera's model. If true, assignments to summary tasks are skipped during export. If false (the default value), an exception will be thrown if assignment to a summary task is encountered during export.

### See Also

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


