---
title: VbaModule.CreateProceduralModule
second_title: Aspose.Tasks for .NET API Reference
description: VbaModule method. Creates an instance of VbaModule with VbaModuleType.ProceduralModule type
type: docs
weight: 20
url: /net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

Creates an instance of [`VbaModule`](../) with VbaModuleType.ProceduralModule type.

```csharp
public static VbaModule CreateProceduralModule(string name)
```

## Examples

Shows how to add/delete VBA macros to/from the existing VbaProject in MPP file.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

            var newModule = VbaModule.CreateProceduralModule("Module20");
            newModule.SourceCode = @"Sub TestMacro()
#If conUnicode Then
Dim p As Project
Set p = Application.ActiveProject
MsgBox ""This is a message from a new macro. Current project: "" & p.Name
#End If
End Sub

Private Sub Project_BeforePrint(ByVal pj As Project)

End Sub";
            project.VbaProject.Modules.Add(newModule);

            var moduleToDelete = project.VbaProject.Modules["EventCode"];
            project.VbaProject.Modules.Remove(moduleToDelete);

            project.Save(OutDir + "VbaProject.AddedModule.mpp", new MPPSaveOptions() { WriteVba = true });
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


