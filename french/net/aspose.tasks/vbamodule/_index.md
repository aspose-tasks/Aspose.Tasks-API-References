---
title: "Classe VbaModule"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.VbaModule. Représente un module VBA."
type: docs
weight: 2810
url: /fr/net/aspose.tasks/vbamodule/
---
## VbaModule class

Représente un module VBA.

```csharp
public sealed class VbaModule
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Obtient une collection des attributs du module. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Obtient le nom du module VBA. |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Obtient ou définit le code source du module VBA. |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Obtient le type du module. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Crée une instance de `VbaModule` avec le type VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Crée une instance de `VbaModule` avec le type VbaModuleType.ProceduralModule. |

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


