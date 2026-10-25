---
title: "Kelas CalendarCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.CalendarCollection. Mewakili kumpulan objek Calendar"
type: docs
weight: 240
url: /id/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Mewakili kumpulan objek [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek `CalendarCollection` ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Menambahkan kalender dasar baru ke objek CalendarCollection ini dan mengembalikan kalender yang ditambahkan. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Menambahkan kalender baru dengan kalender dasar yang ditentukan ke objek CalendarCollection ini dan mengembalikan kalender yang ditambahkan. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Mengembalikan kalender dengan nama yang ditentukan. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Mengembalikan kalender dengan UID yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Menghapus Calendar dari Project CalendarCollection. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Mengonversi objek CalendarCollection menjadi daftar objek [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


