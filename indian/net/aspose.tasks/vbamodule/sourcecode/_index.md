---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModule प्रॉपर्टी। VBA मॉड्यूल का स्रोत कोड प्राप्त करता है या सेट करता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

VBA मॉड्यूल का स्रोत कोड प्राप्त करता है या सेट करता है

```csharp
public string SourceCode { get; set; }
```

## उदाहरण

दिखाता है कि VBA प्रोजेक्ट के मॉड्यूल कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


