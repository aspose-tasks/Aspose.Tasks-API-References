---
title: "Classe VbaModuleAttribute"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.VbaModuleAttribute. L'attribut de l'objet VbaModule"
type: docs
weight: 2820
url: /fr/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

L'attribut de l'objet [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Obtient la clé de l'attribut du module VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Obtient la valeur de l'attribut du module VBA. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à l'objet `VbaModuleAttribute` spécifié. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Renvoie une valeur indiquant si cette instance est égale à l'objet `VbaModuleAttribute` spécifié. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Renvoie une valeur de code de hachage pour ce `VbaModuleAttribute`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


