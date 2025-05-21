---
title: PrimaveraSaveOptions.SkipSummaryAssignments
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraSaveOptions property. Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export
type: docs
weight: 60
url: /net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Remarks

Primavera software doesn't support assignments of resources to summary (WBS) tasks. Thus, export of such assignments can result in an invalid file according to Primavera's model. If true, assignments to summary tasks are skipped during export. If false (the default value), an exception will be thrown if assignment to a summary task is encountered during export.

## Examples

Shows how to use SkipSummaryAssignments flag.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera doesn't support assignments of resources to summary tasks.
// So exporting such assignments to Primavera format may result in files that cannot be imported to Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### See Also

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


