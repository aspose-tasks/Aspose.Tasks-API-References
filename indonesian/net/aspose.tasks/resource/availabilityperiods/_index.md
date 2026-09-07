---
title: "Resource.AvailabilityPeriods"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan instance dari kelas AvailabilityPeriodCollection. Kumpulan periode selama sumber daya tersedia"
type: docs
weight: 130
url: /id/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Mendapatkan instance dari kelas [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). Kumpulan periode selama sumber daya tersedia.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Contoh

Menampilkan cara menambahkan periode ketersediaan untuk sebuah sumber daya.

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

### Lihat Juga

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


