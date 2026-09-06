---
title: "IVbaModule.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété IVbaModule. Obtient le nom du module VBA"
type: docs
weight: 20
url: /fr/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Obtient le nom du module VBA.

```csharp
public string Name { get; }
```

## Exemples

Montre comment lire les modules du projet VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Voir aussi

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


