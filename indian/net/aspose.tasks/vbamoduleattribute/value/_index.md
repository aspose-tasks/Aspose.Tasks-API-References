---
title: "VbaModuleAttribute.Value"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModuleAttribute प्रॉपर्टी। VBA मॉड्यूल एट्रिब्यूट का मान प्राप्त करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

VBA मॉड्यूल एट्रिब्यूट का मान प्राप्त करता है।

```csharp
public string Value { get; }
```

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

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


