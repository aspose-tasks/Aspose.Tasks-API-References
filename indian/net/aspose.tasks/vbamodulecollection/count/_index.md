---
title: "VbaModuleCollection.Count"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleCollection प्रॉपर्टी।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

## उदाहरण

दिखाता है कि VBA मॉड्यूल पर कैसे पुनरावृत्ति करें।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### संबंधित देखें

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


