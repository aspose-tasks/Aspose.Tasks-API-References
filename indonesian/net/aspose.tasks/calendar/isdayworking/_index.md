---
title: "Calendar.IsDayWorking"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender"
type: docs
weight: 260
url: /id/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | DateTime | Tanggal untuk memeriksa apakah hari tersebut bekerja. |

### Nilai Kembali

Benar jika hari tersebut adalah hari kerja.

## Contoh

Menampilkan cara menghitung jam kerja.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Akses Tugas Berdasarkan Id
var task = project.RootTask.Children.GetById(1);

// Akses Kalender dan tanggal mulai serta akhir
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Akses sumber daya dan kalender mereka
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Dapatkan Durasi dalam Menit
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Dapatkan Durasi dalam Jam
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Dapatkan Durasi dalam Hari
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


