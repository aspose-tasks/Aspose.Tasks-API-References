---
title: "VbaModule.CreateClassModule"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModule मेथड। VbaModuleType.ClassModule प्रकार के साथ VbaModule का एक इंस्टेंस बनाता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

[`VbaModule`](../) का एक इंस्टेंस VbaModuleType.ClassModule प्रकार के साथ बनाता है।

```csharp
public static VbaModule CreateClassModule(string name)
```

## उदाहरण

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


