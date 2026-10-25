---
title: "VbaModuleCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "VbaModuleCollection метод. Преобразует объект коллекции в список объектов VbaModule"
type: docs
weight: 100
url: /ru/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Преобразует объект коллекции в список объектов [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### Возвращаемое значение

Список объектов.

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


