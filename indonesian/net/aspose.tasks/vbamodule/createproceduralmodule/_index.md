---
title: "VbaModule.CreateProceduralModule"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode VbaModule. Membuat instance VbaModule dengan tipe VbaModuleType.ProceduralModule"
type: docs
weight: 20
url: /id/net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

Membuat instance dari [`VbaModule`](../) dengan tipe VbaModuleType.ProceduralModule.

```csharp
public static VbaModule CreateProceduralModule(string name)
```

## Contoh

Menampilkan cara menambah/menghapus makro VBA ke/dari VbaProject yang ada dalam file MPP.

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

### Lihat Juga

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


