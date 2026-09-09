---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModule özelliği. VBA modülünün kaynak kodunu alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

VBA modülünün kaynak kodunu alır veya ayarlar

```csharp
public string SourceCode { get; set; }
```

## Örnekler

VBA projesinin modüllerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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


