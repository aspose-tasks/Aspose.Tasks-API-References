---
title: "क्लास VbaModuleCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaModuleCollection क्लास। VbaModule ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 2840
url: /hi/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

[`VbaModule`](../vbamodule/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | निर्दिष्ट अनुक्रमणिका पर मॉड्यूल प्राप्त करता है। (2 इंडेक्सर) |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | संग्रह ऑब्जेक्ट को [`VbaModule`](../vbamodule/) ऑब्जेक्ट्स की सूची में बदलता है। |

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

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


