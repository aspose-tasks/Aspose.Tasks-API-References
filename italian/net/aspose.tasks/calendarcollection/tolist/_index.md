---
title: "CalendarCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarCollection. Converte l'oggetto CalendarCollection in un elenco di oggetti Calendar."
type: docs
weight: 70
url: /it/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Converte l'oggetto CalendarCollection in un elenco di oggetti [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Valore di ritorno

Elenco di oggetti [`Calendar`](../../calendar/).

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


