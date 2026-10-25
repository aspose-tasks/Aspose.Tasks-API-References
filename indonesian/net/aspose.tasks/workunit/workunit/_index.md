---
title: "WorkUnit.WorkUnit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor WorkUnit. Menginisialisasi instance baru dari kelas WorkUnit. Membuat objek WorkUnit baru dengan tanggal From dan To yang ditentukan"
type: docs
weight: 10
url: /id/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Menginisialisasi instance baru dari kelas [`WorkUnit`](../). Membuat objek WorkUnit baru dengan tanggal From dan To yang ditentukan.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| from | DateTime | Tanggal mulai jam kerja. |
| sampai | DateTime | Tanggal selesai jam kerja. |

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

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


