---
title: "VbaModuleCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaModuleCollection."
type: docs
weight: 80
url: /el/net/aspose.tasks/vbamodulecollection/getenumerator/
---
## VbaModuleCollection.GetEnumerator method

```csharp
public IEnumerator<VbaModule> GetEnumerator()
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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


