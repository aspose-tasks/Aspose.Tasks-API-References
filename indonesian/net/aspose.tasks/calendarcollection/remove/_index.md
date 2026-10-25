---
title: "CalendarCollection.Remove"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "metode CalendarCollection. Menghapus Kalender dari Project CalendarCollection"
type: docs
weight: 60
url: /id/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Menghapus Calendar dari Project CalendarCollection.

```csharp
public bool Remove(Calendar item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | Calendar | Kalender yang akan dihapus. |

### Nilai Kembali

Jika dihapus mengembalikan true, jika tidak mengembalikan false.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| InvalidOperationException | Dilemparkan ketika kalender tidak dapat dihapus. |

## Contoh

Menunjukkan cara mengganti kalender dalam koleksi.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// tambahkan kalender baru
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


