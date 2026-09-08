---
title: "IVbaModule.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство IVbaModule. Возвращает имя VBA‑модуля"
type: docs
weight: 20
url: /ru/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Получает имя модуля VBA

```csharp
public string Name { get; }
```

## Примеры

Показывает, как читать модули проекта VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### См. также

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


