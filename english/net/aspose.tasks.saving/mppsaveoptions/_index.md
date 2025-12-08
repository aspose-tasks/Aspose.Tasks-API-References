---
title: Class MPPSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.MPPSaveOptions class. Allows to specify additional options when saving project data to MPP
type: docs
weight: 2020
url: /net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Allows to specify additional options when saving project data to MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Initializes a new instance of the `MPPSaveOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Gets or sets a value indicating whether to remove existing VBA macros data when saving a project to MPP format. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Gets or sets a password which is used to protect a resulting MPP file. Currently is supported for MS Project 2010 and newer formats. Null value indicates that the project file is not protected. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Gets or sets a value indicating whether to remove invalid resource assignments when saving to MPP. MS Project creates an empty resource assignment for each task. Set this flag to true to remove them on save. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Gets or sets a value indicating whether to write filter data when saving a project to MPP for format. Filter data includes Project.TaskFilters and Project.ResourceFilters collections. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Gets or sets a value indicating whether to write groups data when saving a project to MPP for format. Group data includes Project.TaskGroups and Project.ResourceGroups collections. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Gets or sets a value indicating whether to update existing VBA macros data in MPP file. Currently writing of VbaModule.SourceCode is supported. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Gets or sets a value indicating whether to write view data when saving a project to MPP format. View data includes Project.Views, Filters and Tables collections. |

## Examples

Shows how to save project into a stream as an MPP file.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // create save options
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // sets a value indicating whether to remove invalid resource assignments when saving to MPP
        RemoveInvalidAssignments = true
    };

    // save MPP with options
    project.Save(stream, options);
}
```

### See Also

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


