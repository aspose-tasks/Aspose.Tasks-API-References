---
title: "CalendarCollection.GetByUid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarCollection. Restituisce un calendario con l'UID specificato"
type: docs
weight: 40
url: /it/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Restituisce un calendario con l'UID specificato.

```csharp
public Calendar GetByUid(int uid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | Int32 | UID di un calendario. |

### Valore di ritorno

Calendario con un UID specificato.

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


