---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModuleCollection methode. Converteert het collectie‑object naar een lijst van VbaModule‑objecten."
type: docs
weight: 100
url: /nl/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Converteert het collectie‑object naar een lijst van [`VbaModule`](../../vbamodule/) objecten.

```csharp
public List<VbaModule> ToList()
```

### Retourwaarde

Lijst van objecten.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


