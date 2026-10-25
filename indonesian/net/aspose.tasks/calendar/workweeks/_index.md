---
title: "Calendar.WorkWeeks"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan objek WorkWeekCollections. Kumpulan minggu kerja yang terkait dengan kalender"
type: docs
weight: 130
url: /id/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Mendapatkan objek WorkWeekCollections. Kumpulan minggu kerja yang terkait dengan kalender.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Contoh

Menampilkan cara membaca informasi minggu kerja.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Tampilkan nama minggu kerja, tanggal mulai dan selesai
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Data ini semua tentang tombol "Details." Anda dapat mengatur waktu kerja khusus untuk Hari Kerja khusus atau bahkan menjadikannya tidak bekerja.
    foreach (var day in workWeek.WeekDays)
    {
        // Anda dapat menelusuri lebih lanjut melalui waktu kerja dan menampilkannya.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Lihat Juga

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


