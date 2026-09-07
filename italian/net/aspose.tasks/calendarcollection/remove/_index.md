---
title: "CalendarCollection.Remove"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarCollection. Rimuove il Calendario dalla CalendarCollection del Progetto"
type: docs
weight: 60
url: /it/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Rimuove il calendario dalla CalendarCollection del progetto.

```csharp
public bool Remove(Calendar item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | Calendar | Il calendario da rimuovere. |

### Valore di ritorno

Se rimosso restituisce true, altrimenti restituisce false.

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generata quando il calendario non può essere rimosso. |

## Esempi

Mostra come sostituire un calendario nella collezione.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// aggiungi nuovo calendario
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


