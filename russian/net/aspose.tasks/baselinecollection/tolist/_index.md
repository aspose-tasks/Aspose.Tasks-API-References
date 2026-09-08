---
title: "BaselineCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод BaselineCollection. Преобразует объект BaselineCollection в список объектов Baseline"
type: docs
weight: 70
url: /ru/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Преобразует объект BaselineCollection в список объектов [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### Возвращаемое значение

Список объектов [`Baseline`](../../baseline/).

## Примеры

Показывает, как работать с коллекциями baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// читать информацию о baseline
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### См. также

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


