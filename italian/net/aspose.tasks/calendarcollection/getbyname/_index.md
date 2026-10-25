---
title: "CalendarCollection.GetByName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarCollection. Restituisce un calendario con il nome specificato."
type: docs
weight: 30
url: /it/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Restituisce un calendario con il nome specificato.

```csharp
public Calendar GetByName(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | Stringa | Nome di un calendario. |

### Valore di ritorno

Se trovato, restituisce il calendario con il nome specificato, altrimenti restituisce null.

## Esempi

Mostra come ottenere i calendari per nome o per ID.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Vedi anche

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


