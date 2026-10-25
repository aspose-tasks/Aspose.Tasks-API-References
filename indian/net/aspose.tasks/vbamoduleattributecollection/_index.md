---
title: "क्लास VbaModuleAttributeCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaModuleAttributeCollection क्लास। VbaModuleAttribute ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 2830
url: /hi/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

[`VbaModuleAttribute`](../vbamoduleattribute/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## उदाहरण

VBA मॉड्यूल के एट्रिब्यूट संग्रह पर इटरेट करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### संबंधित देखें

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


