---
title: MPPSaveOptions.WriteViewData
second_title: Aspose.Tasks for .NET API Reference
description: MPPSaveOptions property. Gets or sets a value indicating whether to write view data when saving a project to MPP format. View data includes Project.Views Filters and Tables collections
type: docs
weight: 80
url: /net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Gets or sets a value indicating whether to write view data when saving a project to MPP format. View data includes Project.Views, Filters and Tables collections.

```csharp
public bool WriteViewData { get; set; }
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


