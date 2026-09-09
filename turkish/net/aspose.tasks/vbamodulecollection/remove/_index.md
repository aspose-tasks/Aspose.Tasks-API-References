---
title: "VbaModuleCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleCollection yöntemi."
type: docs
weight: 90
url: /tr/net/aspose.tasks/vbamodulecollection/remove/
---
## VbaModuleCollection.Remove method

```csharp
public bool Remove(VbaModule item)
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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


