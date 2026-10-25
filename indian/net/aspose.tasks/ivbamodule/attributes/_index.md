---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "IVbaModule प्रॉपर्टी। VbaModuleAttributeCollection का संग्रह प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

[`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/) का संग्रह प्राप्त करता है।

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


