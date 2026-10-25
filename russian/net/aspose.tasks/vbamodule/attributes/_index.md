---
title: "VbaModule.Attributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaModule. Получает коллекцию атрибутов модуля"
type: docs
weight: 30
url: /ru/net/aspose.tasks/vbamodule/attributes/
---
## VbaModule.Attributes property

Получает коллекцию атрибутов модуля.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## Примеры

Показывает, как читать атрибуты модуля VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### См. также

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


