---
title: "Класс VbaModuleAttribute"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.VbaModuleAttribute. Атрибут объекта VbaModule"
type: docs
weight: 2820
url: /ru/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

Атрибут объекта [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Получает ключ атрибута модуля VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Получает значение атрибута модуля VBA. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту `VbaModuleAttribute`. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту `VbaModuleAttribute`. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Возвращает значение хеш‑кода для этого `VbaModuleAttribute`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


