---
title: "Calendar.Make24HourCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Membuat Calendar tertentu menjadi Calendar 24Jam. Calendar 24Jam adalah Calendar di mana setiap hari dalam seminggu bekerja dengan jam kerja 24 jam."
type: docs
weight: 10
url: /id/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Membuat Calendar tertentu menjadi Calendar 24Jam. Calendar 24Jam adalah Calendar di mana setiap hari dalam seminggu bekerja dengan jam kerja 24/7.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kalender | Calendar | Kalender untuk membuat Kalender 24 Jam dari. |

### Nilai Kembali

Kalender 24 Jam.

## Contoh

Menampilkan cara membuat kalender 24 jam.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 jam akan dicetak
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Menampilkan cara mengubah kalender baru menjadi kalender 24 jam.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 jam akan dicetak
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


