---
title: "CalendarCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "properti CalendarCollection. Mendapatkan jumlah objek yang terkandung dalam objek CalendarCollection ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Mendapatkan jumlah objek yang terkandung dalam objek [`CalendarCollection`](../) ini.

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


