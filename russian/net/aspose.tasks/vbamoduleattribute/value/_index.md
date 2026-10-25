---
title: "VbaModuleAttribute.Value"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaModuleAttribute. Получает значение атрибута модуля VBA."
type: docs
weight: 20
url: /ru/net/aspose.tasks/vbamoduleattribute/value/
---
## VbaModuleAttribute.Value property

Получает значение атрибута модуля VBA.

```csharp
public string Value { get; }
```

## Примеры

Показывает, как работать с атрибутами модуля VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### См. также

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


