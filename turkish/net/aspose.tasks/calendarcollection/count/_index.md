---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection özelliği. Bu CalendarCollection nesnesinde bulunan nesne sayısını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Bu [`CalendarCollection`](../) nesnesinde bulunan nesne sayısını alır.

```csharp
public int Count { get; }
```

## Örnekler

Takvim koleksiyonunda nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ayrıca Bakınız

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


