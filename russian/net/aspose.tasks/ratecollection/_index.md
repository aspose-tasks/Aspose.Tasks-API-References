---
title: "Класс RateCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.RateCollection. Представляет коллекцию, содержащую объекты Rate."
type: docs
weight: 1630
url: /ru/net/aspose.tasks/ratecollection/
---
## RateCollection class

Представляет коллекцию, содержащую объекты [`Rate`](../rate/).

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Возвращает количество элементов, содержащихся в RateCollection. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Получает родительский объект [`Resource`](../resource/) для этой коллекции. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Добавляет новый экземпляр [`Rate`](../rate/) в эту коллекцию. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Добавляет новый экземпляр [`Rate`](../rate/) в эту коллекцию. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Удаляет экземпляр Rate из этой коллекции. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Преобразует объект `RateCollection` в список объектов [`Rate`](../rate/). |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Преобразует объект `RateCollection` в список объектов [`Rate`](../rate/), отфильтрованных по указанному типу [`RateType`](../ratetype/). |

## Примеры

Показывает, как работать с коллекциями ставок.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// получить последнюю ставку через доступ по индексу
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// работать со ставками
// ...

// удалить все ставки типа A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// преобразовать коллекцию ставок в плоский список
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### См. также

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


