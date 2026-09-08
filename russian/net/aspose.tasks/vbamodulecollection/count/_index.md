---
title: "VbaModuleCollection.Count"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "VbaModuleCollection свойство."
type: docs
weight: 10
url: /ru/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

## Примеры

Показывает, как перебрать модули VBA.

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

### См. также

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


