---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Takvimin temel takvim (baseline) olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Takvimin temel çizgi takvimi olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Örnekler

Bir takvimin temel takvim olup olmadığını kontrol etmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


