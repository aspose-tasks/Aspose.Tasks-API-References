---
title: "CalendarCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection-eigenschap. Haalt het aantal objecten op dat in dit CalendarCollection-object zit"
type: docs
weight: 10
url: /nl/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Haalt het aantal objecten op dat in dit [`CalendarCollection`](../)-object zit.

```csharp
public int Count { get; }
```

## Voorbeelden

Toont hoe je over de agenda-collectie iterereert.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Zie ook

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


