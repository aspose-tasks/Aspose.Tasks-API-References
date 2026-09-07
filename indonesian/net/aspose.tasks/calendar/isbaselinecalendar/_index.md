---
title: "Calendar.IsBaselineCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan atau mengatur nilai yang menunjukkan apakah kalender adalah kalender baseline"
type: docs
weight: 80
url: /id/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Mendapatkan atau mengatur nilai yang menunjukkan apakah kalender adalah kalender baseline.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Contoh

Menampilkan cara memeriksa apakah kalender adalah kalender baseline atau tidak.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


