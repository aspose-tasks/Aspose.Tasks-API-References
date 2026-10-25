---
title: "Calendar.Uid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan atau mengatur pengidentifikasi unik kalender"
type: docs
weight: 110
url: /id/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Mendapatkan atau mengatur pengidentifikasi unik kalender.

```csharp
public int Uid { get; set; }
```

## Contoh

Menampilkan cara mengambil info kalender.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Ambil Informasi Kalender
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


