---
title: "Kaynak.AvailabilityPeriods"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Kaynak özelliği. AvailabilityPeriodCollection sınıfının bir örneğini alır. Bir kaynağın mevcut olduğu dönemlerin koleksiyonu"
type: docs
weight: 130
url: /tr/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

[`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) sınıfının bir örneğini alır. Bir kaynağın mevcut olduğu dönemlerin koleksiyonu.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Örnekler

Bir kaynak için kullanılabilirlik dönemi eklemenin nasıl yapılacağını gösterir.

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

### Ayrıca Bakınız

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


