---
title: "IVbaModule.Attributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété IVbaModule. Obtient une collection de VbaModuleAttributeCollection"
type: docs
weight: 10
url: /fr/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Obtient une collection de [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Exemples

Montre comment lire les attributs du module VBA.

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

### Voir aussi

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


