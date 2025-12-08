---
title: Class PrimaveraXmlSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PrimaveraXmlSaveOptions class. Allows to specify additional options when saving project to Primavera xml format
type: docs
weight: 2130
url: /net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Allows to specify additional options when saving project to Primavera xml format.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Initializes a new instance of the `PrimaveraXmlSaveOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Gets or sets a value indicating whether to save a root task or not. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |

## Examples

Shows how to export the to Primavera XML file.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### See Also

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


