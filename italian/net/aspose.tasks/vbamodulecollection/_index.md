---
title: "Classe VbaModuleCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.VbaModuleCollection. Rappresenta una raccolta di oggetti VbaModule"
type: docs
weight: 2840
url: /it/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

Rappresenta una raccolta di oggetti [`VbaModule`](../vbamodule/).

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | Ottiene il modulo all'indice specificato. (2 indicizzatori) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | Converte l'oggetto raccolta in un elenco di oggetti [`VbaModule`](../vbamodule/). |

## Esempi

Mostra come iterare sui moduli VBA.

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

### Vedi anche

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


