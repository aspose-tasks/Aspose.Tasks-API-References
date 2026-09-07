---
title: "VbaModuleCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "VbaModuleCollection metodo. Converte l'oggetto della raccolta in un elenco di oggetti VbaModule"
type: docs
weight: 100
url: /it/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Converte l'oggetto della raccolta in un elenco di oggetti [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### Valore di ritorno

Elenco di oggetti.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


