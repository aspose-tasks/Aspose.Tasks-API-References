---
title: "Resource.Baselines"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает экземпляр BaselineCollection для этого объекта. Базовые значения для ресурса"
type: docs
weight: 160
url: /ru/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Получает экземпляр BaselineCollection для этого объекта. Базовые значения для ресурса.

```csharp
public BaselineCollection Baselines { get; }
```

## Примеры

Показывает, как читать базовые линии ресурса.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### См. также

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


