---
title: "WorkUnit.From"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti WorkUnit. Mendapatkan atau mengatur tanggal From"
type: docs
weight: 20
url: /id/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Mendapatkan atau mengatur tanggal From.

```csharp
public DateTime From { get; set; }
```

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


