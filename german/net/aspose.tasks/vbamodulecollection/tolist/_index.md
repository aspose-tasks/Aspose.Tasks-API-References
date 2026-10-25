---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "VbaModuleCollection-Methode. Konvertiert das Sammlungsobjekt in eine Liste von VbaModule-Objekten"
type: docs
weight: 100
url: /de/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Konvertiert das Sammlungsobjekt in eine Liste von [`VbaModule`](../../vbamodule/) Objekten.

```csharp
public List<VbaModule> ToList()
```

### Rückgabewert

Liste von Objekten.

## Beispiele

Zeigt, wie man über VBA-Module iteriert.

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

### Siehe auch

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


