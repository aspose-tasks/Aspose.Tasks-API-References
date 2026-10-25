---
title: "CalendarCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "metode CalendarCollection. Mengonversi objek CalendarCollection menjadi daftar objek Calendar."
type: docs
weight: 70
url: /id/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Mengonversi objek CalendarCollection menjadi daftar objek [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Nilai Kembali

Daftar objek [`Calendar`](../../calendar/).

## Contoh

Menunjukkan cara mengiterasi koleksi kalender.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Lihat Juga

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


