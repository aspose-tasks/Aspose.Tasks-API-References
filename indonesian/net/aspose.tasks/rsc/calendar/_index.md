---
title: "Rsc.Calendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Kalender sebuah sumber daya"
type: docs
weight: 190
url: /id/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Kalender sumber daya.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Contoh

Menampilkan cara mendapatkan/mengatur kalender sumber daya.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Tambahkan kalender standar dan tugaskan ke sumber daya
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Tampilkan nama kalender dasar untuk semua sumber daya
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


