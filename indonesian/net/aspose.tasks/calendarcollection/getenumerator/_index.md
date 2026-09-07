---
title: "CalendarCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "metode CalendarCollection. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 50
url: /id/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

## Contoh

Menampilkan cara menambahkan kalender baru.

```csharp
var project = new Project();

// Kalender baru dapat ditambahkan ke koleksi kalender proyek dengan menggunakan overload Add pada koleksi.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


