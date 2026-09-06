---
title: "IVbaModule.SourceCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété IVbaModule. Obtient le code source du module VBA"
type: docs
weight: 30
url: /fr/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Obtient le code source du module VBA

```csharp
public string SourceCode { get; }
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


