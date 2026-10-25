---
title: "Calendar.GetIntersectionCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Mendapatkan instance ICalendar yang dapat digunakan untuk melakukan perhitungan pada irisan jadwal kerja dari 2 kalender"
type: docs
weight: 280
url: /id/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Mendapatkan instance [`ICalendar`](../../icalendar/) yang dapat digunakan untuk melakukan perhitungan pada irisan jadwal kerja dari 2 kalender.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| calendar1 | Calendar | Kalender pertama. |
| calendar2 | Calendar | Kalender kedua. |

### Nilai Kembali

Implementasi antarmuka ICalendar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Ketika salah satu argumen bernilai null. |

## Contoh

Menampilkan cara menggunakan metode Calendar.GetIntersectionCalendar() untuk melakukan perhitungan pada kalender penugasan.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### Lihat Juga

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


