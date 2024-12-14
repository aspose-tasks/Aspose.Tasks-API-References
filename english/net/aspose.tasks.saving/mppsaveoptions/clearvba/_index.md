---
title: MPPSaveOptions.ClearVba
second_title: Aspose.Tasks for .NET API Reference
description: MPPSaveOptions property. Gets or sets a value indicating whether to remove existing VBA macros data when saving a project to MPP format
type: docs
weight: 20
url: /net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Gets or sets a value indicating whether to remove existing VBA macros data when saving a project to MPP format.

```csharp
public bool ClearVba { get; set; }
```

## Examples

Shows how to remove VBA macros from MPP file.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### See Also

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


