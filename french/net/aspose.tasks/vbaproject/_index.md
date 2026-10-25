---
title: "Classe VbaProject"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.VbaProject. Représente VbaProject."
type: docs
weight: 2860
url: /fr/net/aspose.tasks/vbaproject/
---
## VbaProject class

Représente `VbaProject`.

```csharp
public class VbaProject
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Obtient les arguments de compilation conditionnelle |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Obtient une description du projet. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Obtient l'identifiant de contexte d'aide du projet |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Obtient le nom du fichier d'aide |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Obtient une collection de [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Obtient le nom du projet |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Obtient une collection de [`VbaReferenceCollection`](../vbareferencecollection/) |

## Exemples

Montre comment lire les propriétés du projet VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


