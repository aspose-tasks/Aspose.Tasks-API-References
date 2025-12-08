---
title: Class PrimaveraSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.PrimaveraSaveOptions class. Allows to specify additional options when saving project to Primavera XER format
type: docs
weight: 2120
url: /net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Allows to specify additional options when saving project to Primavera XER format.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Initializes a new instance of the `PrimaveraSaveOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Gets or sets the increment used in renumbering of activity IDs. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Gets or sets the prefix used in renumbering of activity IDs. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Gets or sets the suffix used in renumbering of activity IDs. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Gets or sets a value indicating whether is need to renumbers activity IDs. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Gets or sets a value indicating whether assignments of resources to summary tasks should be skipped during export. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |

## Examples

Shows how to work with &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// create Primavera save options and tune them
var options = new PrimaveraSaveOptions
                  {
                      // define prefix and suffix of an activity
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // control renumbering of activities
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### See Also

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


