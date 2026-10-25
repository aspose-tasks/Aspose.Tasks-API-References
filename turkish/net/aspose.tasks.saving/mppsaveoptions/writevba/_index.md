---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MPPSaveOptions özelliği. MPP dosyasındaki mevcut VBA makro verilerinin güncellenip güncellenmeyeceğini gösteren bir değeri alır veya ayarlar. Şu anda VbaModule.SourceCode yazımı desteklenmektedir."
type: docs
weight: 70
url: /tr/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

MPP dosyasındaki mevcut VBA makro verilerini güncelleyip güncellemeyeceğini gösteren bir değeri alır veya ayarlar. Şu anda VbaModule.SourceCode yazımı desteklenmektedir.

```csharp
public bool WriteVba { get; set; }
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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


