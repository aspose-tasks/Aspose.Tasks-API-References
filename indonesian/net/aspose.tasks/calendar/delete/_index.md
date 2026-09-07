---
title: "Calendar.Delete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Menghapus kalender dari proyek"
type: docs
weight: 140
url: /id/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Menghapus kalender dari proyek.

```csharp
public void Delete()
```

## Contoh

Menampilkan cara menghapus kalender dari proyek.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// dapatkan kalender berdasarkan nama
var calendar = project.Calendars.GetByName("Broken Calendar");

// hapus kalender
calendar.Delete();
```

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


