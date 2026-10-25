---
title: "VbaModule.Attributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaModule. Obtient une collection des attributs du module"
type: docs
weight: 30
url: /fr/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Obtient une collection des attributs du module.

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
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


