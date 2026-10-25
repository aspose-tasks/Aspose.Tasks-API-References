---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Calcola l'inizio del prossimo giorno lavorativo per la data specificata"
type: docs
weight: 180
url: /it/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Calcola l'inizio del prossimo giorno lavorativo per la data specificata.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | DateTime | La data per cui ottenere l'inizio del prossimo giorno lavorativo. |

### Valore di ritorno

Data/Ora di inizio del prossimo giorno lavorativo.

## Esempi

Mostra come ottenere l'inizio del prossimo giorno lavorativo usando un calendario.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni l'inizio del prossimo giorno lavorativo (il fine settimana è saltato)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 aprile 2020 09:00 verrà stampato
Console.WriteLine(nextWorkingDayStart);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


