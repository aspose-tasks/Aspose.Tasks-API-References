---
title: "WeekDay.Clone"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode WeekDay. Mengembalikan salinan mendalam dari hari dalam seminggu"
type: docs
weight: 80
url: /id/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Mengembalikan salinan mendalam dari hari kerja.

```csharp
public WeekDay Clone()
```

### Nilai Kembali

Mengembalikan salinan mendalam dari hari dalam seminggu.

## Contoh

Menunjukkan cara mengkloning hari dalam seminggu.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// buat salinan mendalam hari dalam seminggu
var weekDay2 = weekDay1.Clone();

// Kesetaraan kalender diperiksa terhadap properti weekday:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Lihat Juga

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


