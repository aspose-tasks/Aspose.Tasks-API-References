---
title: "CalendarCollection.Count"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CalendarCollection. Ottiene il numero di oggetti contenuti in questo oggetto CalendarCollection"
type: docs
weight: 10
url: /it/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Ottiene il numero di oggetti contenuti in questo oggetto [`CalendarCollection`](../).

```csharp
public int Count { get; }
```

## Esempi

Mostra come iterare sulla collezione di calendari.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Vedi anche

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


