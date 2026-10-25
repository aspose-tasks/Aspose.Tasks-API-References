---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Membuat Calendar yang diberikan menjadi Night Shift Calendar"
type: docs
weight: 20
url: /id/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Membuat Kalender yang diberikan menjadi Kalender Shift Malam.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kalender | Calendar | Calendar untuk membuat Night Shift Calendar. |

### Nilai Kembali

Night Shift Calendar.

## Contoh

Menampilkan cara membuat night shift calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// tampilkan jam kerja
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Menampilkan cara mengubah kalender menjadi night shift calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// tampilkan jam kerja
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


