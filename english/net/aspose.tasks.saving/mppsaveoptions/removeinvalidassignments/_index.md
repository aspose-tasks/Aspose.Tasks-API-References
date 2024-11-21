---
title: MPPSaveOptions.RemoveInvalidAssignments
second_title: Aspose.Tasks for .NET API Reference
description: MPPSaveOptions property. Gets or sets a value indicating whether to remove invalid resource assignments when saving to MPP. MS Project creates an empty resource assignment for each task. Set this flag to true to remove them on save
type: docs
weight: 40
url: /net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Gets or sets a value indicating whether to remove invalid resource assignments when saving to MPP. MS Project creates an empty resource assignment for each task. Set this flag to true to remove them on save.

```csharp
public bool RemoveInvalidAssignments { get; set; }
```

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


