---
title: "VbaModule.Attributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "VbaModule प्रॉपर्टी। मॉड्यूल के एट्रिब्यूट्स का संग्रह प्राप्त करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

मॉड्यूल के गुणों का संग्रह प्राप्त करता है।

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## उदाहरण

दिखाता है कि VBA मॉड्यूल के एट्रिब्यूट्स को कैसे पढ़ा जाए।

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### संबंधित देखें

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


