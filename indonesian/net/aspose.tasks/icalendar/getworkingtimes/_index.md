---
title: "ICalendar.GetWorkingTimes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ICalendar. Mengembalikan WorkingTimeCollection dari waktu kerja untuk tanggal yang ditentukan."
type: docs
weight: 80
url: /id/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

Mengembalikan [`WorkingTimeCollection`](../../workingtimecollection/) dari waktu kerja untuk tanggal yang ditentukan.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | DateTime | Tanggal untuk mendapatkan waktu kerja. |

### Nilai Kembali

Koleksi instance [`WorkingTime`](../../workingtime/).

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


