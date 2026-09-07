---
title: "CalendarCollection.GetByUid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "metode CalendarCollection. Mengembalikan kalender dengan UID yang ditentukan"
type: docs
weight: 40
url: /id/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Mengembalikan kalender dengan UID yang ditentukan.

```csharp
public Calendar GetByUid(int uid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | Int32 | UID sebuah kalender. |

### Nilai Kembali

Kalender dengan UID yang ditentukan.

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


