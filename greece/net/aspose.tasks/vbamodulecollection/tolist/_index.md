---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaModuleCollection. Μετατρέπει το αντικείμενο συλλογής σε λίστα αντικειμένων VbaModule"
type: docs
weight: 100
url: /el/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Μετατρέπει το αντικείμενο συλλογής σε λίστα αντικειμένων [`VbaModule`](../../vbamodule/) αντικειμένων.

```csharp
public List<VbaModule> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων.

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


