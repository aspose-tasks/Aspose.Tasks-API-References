---
title: "Класс BaselineCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.BaselineCollection. Представляет коллекцию объектов Baseline"
type: docs
weight: 120
url: /ru/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Представляет коллекцию объектов [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте BaselineCollection. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Получает родительский объект [`Resource`](../resource/) для этой коллекции. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Удаляет базовую линию из этой коллекции. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Преобразует объект BaselineCollection в список объектов [`Baseline`](../baseline/). |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


