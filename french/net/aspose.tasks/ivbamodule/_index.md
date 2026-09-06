---
title: "Interface IVbaModule"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Interface Aspose.Tasks.IVbaModule. Représente un module avec du code VBA"
type: docs
weight: 880
url: /fr/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Représente un module avec du code VBA.

```csharp
public interface IVbaModule
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Obtient une collection de [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Obtient le nom du module VBA. |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Obtient le code source du module VBA |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


