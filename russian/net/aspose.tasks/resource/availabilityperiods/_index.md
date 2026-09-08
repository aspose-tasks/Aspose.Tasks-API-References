---
title: "Resource.AvailabilityPeriods"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает экземпляр класса AvailabilityPeriodCollection. Коллекция периодов, в течение которых ресурс доступен"
type: docs
weight: 130
url: /ru/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Получает экземпляр класса [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). Коллекция периодов, в течение которых ресурс доступен.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Примеры

Показывает, как добавить период доступности для ресурса.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### См. также

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


