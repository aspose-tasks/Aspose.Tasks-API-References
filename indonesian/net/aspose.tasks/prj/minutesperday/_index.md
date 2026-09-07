---
title: "Prj.MinutesPerDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Jumlah menit per hari"
type: docs
weight: 470
url: /id/net/aspose.tasks/prj/minutesperday/
---
## Prj.MinutesPerDay field

Jumlah menit per hari.

```csharp
public static readonly Key<int, PrjKey> MinutesPerDay;
```

## Contoh

Menampilkan cara membaca/menulis properti hari kerja proyek.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Atur properti hari kerja
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Tampilkan properti hari kerja
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


