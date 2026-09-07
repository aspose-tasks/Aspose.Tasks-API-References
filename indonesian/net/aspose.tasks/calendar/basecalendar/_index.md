---
title: "Calendar.BaseCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan atau mengatur kalender dasar yang menjadi dependensi kalender ini. Hanya berlaku jika kalender bukan kalender dasar"
type: docs
weight: 40
url: /id/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Mendapatkan atau mengatur kalender dasar yang menjadi dependensi kalender ini. Hanya berlaku jika kalender bukan kalender dasar.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan kalender dasar dari kalender sumber daya.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Tambahkan kalender standar dan tugaskan ke sumber daya
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Tampilkan nama kalender dasar untuk semua sumber daya
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


