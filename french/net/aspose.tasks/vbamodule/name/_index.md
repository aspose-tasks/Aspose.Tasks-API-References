---
title: "VbaModule.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaModule. Obtient le nom du module VBA"
type: docs
weight: 40
url: /fr/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Obtient le nom du module VBA.

```csharp
public string Name { get; set; }
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


