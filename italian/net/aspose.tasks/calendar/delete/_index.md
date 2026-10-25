---
title: "Calendar.Delete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Rimuove il calendario dal progetto"
type: docs
weight: 140
url: /it/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Rimuove il calendario dal progetto.

```csharp
public void Delete()
```

## Esempi

Mostra come eliminare un calendario da un progetto.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// ottieni il calendario per nome
var calendar = project.Calendars.GetByName("Broken Calendar");

// elimina il calendario
calendar.Delete();
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


