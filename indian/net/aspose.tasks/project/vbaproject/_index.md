---
title: "Project.VbaProject"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। VbaProject क्लास का एक इंस्टेंस प्राप्त करता है"
type: docs
weight: 1010
url: /hi/net/aspose.tasks/project/vbaproject/
---
## Project.VbaProject property

`VbaProject` क्लास का एक इंस्टेंस प्राप्त करता है।

```csharp
public VbaProject VbaProject { get; }
```

## उदाहरण

MPP फ़ाइल से VBA मैक्रो को हटाने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

VBA प्रोजेक्ट जानकारी को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

MPP फ़ाइल में मौजूदा VbaProject में VBA मैक्रो को जोड़ने/हटाने का तरीका दिखाता है।

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

### संबंधित देखें

* class [VbaProject](../../vbaproject/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


