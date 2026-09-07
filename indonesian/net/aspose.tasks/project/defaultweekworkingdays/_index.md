---
title: "Project.DefaultWeekWorkingDays"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan instance kelas WeekDayCollection yang mewakili koleksi hari kerja minggu default proyek dan waktu kerja."
type: docs
weight: 370
url: /id/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Mendapatkan instance kelas [`WeekDayCollection`](../../weekdaycollection/) yang mewakili koleksi hari kerja minggu default proyek dan waktu kerja.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Nilai Kembali

Instance kelas [`WeekDayCollection`](../../weekdaycollection/) yang berisi daftar objek [`WeekDay`](../../weekday/).

## Catatan

Data hanya terdapat dalam file mpp (bukan dalam xml).

## Contoh

Menampilkan cara mendapatkan hari kerja minggu default.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Lihat Juga

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


