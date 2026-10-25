---
title: "Antarmuka ICalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Antarmuka Aspose.Tasks.ICalendar. Mewakili abstraksi kalender yang dapat digunakan untuk berbagai perhitungan tanggal dan durasi."
type: docs
weight: 840
url: /id/net/aspose.tasks/icalendar/
---
## ICalendar interface

Mewakili abstraksi kalender yang dapat digunakan untuk berbagai perhitungan tanggal dan durasi.

```csharp
public interface ICalendar
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Menghitung tanggal dan waktu selesai tugas dari tanggal mulainya, bagian-bagian terpisah, dan durasi kerja. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Mengembalikan jumlah jam kerja pada tanggal yang ditentukan. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Mengembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Mengembalikan jumlah jam kerja antara tanggal yang ditentukan. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Mengembalikan [`WorkingTimeCollection`](../workingtimecollection/) dari waktu kerja untuk tanggal yang ditentukan. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


