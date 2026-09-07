---
title: "Class VbaModuleAttribute"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.VbaModuleAttribute क्लास। VbaModule ऑब्जेक्ट का एट्रिब्यूट"
type: docs
weight: 2820
url: /hi/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

[`VbaModule`](../vbamodule/) ऑब्जेक्ट का एट्रिब्यूट

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | VBA मॉड्यूल एट्रिब्यूट की कुंजी प्राप्त करता है। |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | VBA मॉड्यूल एट्रिब्यूट का मान प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट `VbaModuleAttribute` वस्तु के बराबर है या नहीं। |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | एक मान लौटाता है जो दर्शाता है कि यह उदाहरण निर्दिष्ट `VbaModuleAttribute` वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | इस `VbaModuleAttribute` के लिए हैश कोड मान लौटाता है। |

## उदाहरण

VBA मॉड्यूल एट्रिब्यूट्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


