---
title: "VbaProject.Modules"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaProject प्रॉपर्टी। प्राप्त करता है VbaModuleCollection का संग्रह"
type: docs
weight: 50
url: /hi/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

प्राप्त करता है [`VbaModuleCollection`](../../vbamodulecollection/) का संग्रह

```csharp
public VbaModuleCollection Modules { get; }
```

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट के VBS मॉड्यूल्स पर इटररेट किया जाए।

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

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


