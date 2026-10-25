---
title: "VbaModule.CreateProceduralModule"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModule yöntemi. VbaModuleType.ProceduralModule türüyle bir VbaModule örneği oluşturur."
type: docs
weight: 20
url: /tr/net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

[`VbaModule`](../) örneğini VbaModuleType.ProceduralModule türüyle oluşturur.

```csharp
public static VbaModule CreateProceduralModule(string name)
```

## Örnekler

MPP dosyasındaki mevcut VbaProject'e VBA makrolarını ekleme/silme işlemini nasıl yapacağınızı gösterir.

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

### Ayrıca Bakınız

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


