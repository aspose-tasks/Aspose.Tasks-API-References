---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection-methode. Converteert het CalendarCollection-object naar een lijst van Calendar-objecten."
type: docs
weight: 70
url: /nl/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Converteert het CalendarCollection-object naar een lijst van [`Calendar`](../../calendar/)-objecten.

```csharp
public List<Calendar> ToList()
```

### Retourwaarde

Lijst van [`Calendar`](../../calendar/)-objecten.

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


