---
title: "IVbaModule.Attributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство IVbaModule. Возвращает коллекцию VbaModuleAttributeCollection"
type: docs
weight: 10
url: /ru/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

Возвращает коллекцию [`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)

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
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


