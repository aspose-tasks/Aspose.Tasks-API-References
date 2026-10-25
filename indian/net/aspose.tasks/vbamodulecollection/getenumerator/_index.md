---
title: "VbaModuleCollection.GetEnumerator"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleCollection मेथड।"
type: docs
weight: 80
url: /hi/net/aspose.tasks/vbamodulecollection/getenumerator/
---
## VbaModuleCollection.GetEnumerator method

```csharp
public IEnumerator<VbaModule> GetEnumerator()
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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


