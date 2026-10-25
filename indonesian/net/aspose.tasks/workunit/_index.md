---
title: "Kelas WorkUnit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WorkUnit. Mewakili jam kerja"
type: docs
weight: 3630
url: /id/net/aspose.tasks/workunit/
---
## WorkUnit class

Mewakili jam kerja.

```csharp
public class WorkUnit
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Menginisialisasi instance baru dari kelas `WorkUnit`. Membuat objek WorkUnit baru dengan tanggal From dan To yang ditentukan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Mendapatkan atau mengatur tanggal From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Mendapatkan atau mengatur tanggal To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Mendapatkan atau mengatur durasi jam kerja. |

## Contoh

Menampilkan cara bekerja dengan informasi unit kerja.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// dapatkan jam kerja untuk tanggal tertentu
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


