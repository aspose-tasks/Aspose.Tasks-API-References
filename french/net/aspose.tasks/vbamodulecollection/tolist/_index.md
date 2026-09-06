---
title: "VbaModuleCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaModuleCollection. Convertit l'objet collection en une liste d'objets VbaModule"
type: docs
weight: 100
url: /fr/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Convertit l'objet collection en une liste d'objets [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### Valeur de retour

Liste d'objets.

## Exemples

Montre comment itérer sur les modules VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### Voir aussi

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


