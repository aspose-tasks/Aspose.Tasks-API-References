---
title: "VbaModuleCollection.Count"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "VbaModuleCollection Eigenschaft."
type: docs
weight: 10
url: /de/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

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

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


