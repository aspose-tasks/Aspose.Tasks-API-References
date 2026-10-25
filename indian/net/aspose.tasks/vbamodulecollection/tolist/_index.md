---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleCollection मेथड। संग्रह वस्तु को VbaModule वस्तुओं की सूची में बदलता है"
type: docs
weight: 100
url: /hi/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

संग्रह वस्तु को [`VbaModule`](../../vbamodule/) वस्तुओं की सूची में बदलता है।

```csharp
public List<VbaModule> ToList()
```

### रिटर्न वैल्यू

वस्तुओं की सूची।

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


