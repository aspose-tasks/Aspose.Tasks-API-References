---
title: "VbaModuleCollection.Count"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModuleCollection."
type: docs
weight: 10
url: /el/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις μονάδες VBA.

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

### Δείτε επίσης

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


