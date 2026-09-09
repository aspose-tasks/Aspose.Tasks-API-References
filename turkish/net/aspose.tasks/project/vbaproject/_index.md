---
title: "Project.VbaProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. VbaProject sınıfının bir örneğini alır"
type: docs
weight: 1010
url: /tr/net/aspose.tasks/project/vbaproject/
---
## Project.VbaProject property

`VbaProject` sınıfının bir örneğini alır.

```csharp
public VbaProject VbaProject { get; }
```

## Örnekler

MPP dosyasından VBA makrolarını nasıl kaldıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

VBA proje bilgilerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
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

* class [VbaProject](../../vbaproject/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


