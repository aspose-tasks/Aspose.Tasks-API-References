---
title: "ICalendar.GetWorkingHours"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ICalendar. Mengembalikan WorkUnit Start Finish dan Duration jam kerja untuk interval tanggal dan waktu yang ditentukan."
type: docs
weight: 60
url: /id/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Mengembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | DateTime | Tanggal mulai interval. |
| selesai | DateTime | Tanggal selesai interval. |

### Nilai Kembali

Instance kelas [`WorkUnit`](../../workunit/) yang berisi Start, Finish, dan Duration jam kerja.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Mengembalikan jumlah jam kerja pada tanggal yang ditentukan.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | DateTime | Tanggal untuk mendapatkan jam kerja. |

### Nilai Kembali

Jam kerja pada tanggal yang ditentukan.

### Lihat Juga

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


