---
title: "VbaModule.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaModule. Получает имя модуля VBA"
type: docs
weight: 40
url: /ru/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Получает имя модуля VBA

```csharp
public string Name { get; set; }
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


