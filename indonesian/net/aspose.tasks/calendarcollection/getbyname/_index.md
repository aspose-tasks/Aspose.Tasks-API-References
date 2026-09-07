---
title: "CalendarCollection.GetByName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode CalendarCollection. Mengembalikan kalender dengan nama yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Mengembalikan kalender dengan nama yang ditentukan.

```csharp
public Calendar GetByName(string name)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | String | Nama sebuah kalender. |

### Nilai Kembali

Jika ditemukan, mengembalikan kalender dengan nama yang ditentukan, jika tidak mengembalikan null.

## Contoh

Menampilkan cara mendapatkan kalender berdasarkan nama atau ID.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


