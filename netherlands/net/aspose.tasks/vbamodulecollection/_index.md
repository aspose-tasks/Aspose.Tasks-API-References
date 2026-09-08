---
title: "Klasse VbaModuleCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaModuleCollection klasse. Vertegenwoordigt een verzameling van VbaModule-objecten"
type: docs
weight: 2840
url: /nl/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

Vertegenwoordigt een verzameling van [`VbaModule`](../vbamodule/) objecten.

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | Haalt de module op op de opgegeven index. (2 indexeerders) |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | Converteert het verzamelingsobject naar een lijst van [`VbaModule`](../vbamodule/) objecten. |

## Voorbeelden

Toont hoe over VBA-modules geïtereerd kan worden.

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

### Zie ook

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


