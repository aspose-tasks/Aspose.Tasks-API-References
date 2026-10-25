---
title: "BaselineCollection.Remove"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод BaselineCollection. Удаляет baseline из этой коллекции"
type: docs
weight: 60
url: /ru/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Удаляет базовую линию из этой коллекции.

```csharp
public bool Remove(Baseline item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | Baseline | Элемент для удаления. |

### Возвращаемое значение

true, если экземпляр [`Baseline`](../../baseline/) был успешно удалён; иначе false

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


