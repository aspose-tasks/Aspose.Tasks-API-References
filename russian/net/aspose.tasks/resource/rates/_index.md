---
title: "Resource.Rates"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает экземпляр класса RateCollection для этого объекта. Коллекция периодов и ставок, связанных с каждым из них"
type: docs
weight: 640
url: /ru/net/aspose.tasks/resource/rates/
---
## Resource.Rates property

Получает экземпляр класса [`RateCollection`](../../ratecollection/) для этого объекта. Коллекция периодов и ставок, связанных с каждым из них.

```csharp
public RateCollection Rates { get; }
```

## Примеры

Показывает, как прочитать ставки ресурса.

```csharp
var project = new Project();
var resource = project.Resources.Add();
resource.Set(Rsc.Uid, 1);
resource.Set(Rsc.Name, "Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

// итерация по ставкам
foreach (KeyValuePair<RateType, RateByDateCollection> rate in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in rate.Value)
    {
        Console.WriteLine(pair.Value.RatesFrom);
        Console.WriteLine(pair.Value.RatesTo);
    }
}
```

### См. также

* class [RateCollection](../../ratecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


