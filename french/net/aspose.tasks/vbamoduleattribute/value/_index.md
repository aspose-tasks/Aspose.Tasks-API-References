---
title: "VbaModuleAttribute.Value"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaModuleAttribute. Obtient la valeur de l'attribut de module VBA"
type: docs
weight: 20
url: /fr/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Obtient la valeur de l'attribut du module VBA.

```csharp
public string Value { get; }
```

## Exemples

Montre comment travailler avec les attributs de module VBA.

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

### Voir aussi

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


