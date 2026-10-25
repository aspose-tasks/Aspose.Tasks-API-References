---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Calcola la fine della data lavorativa precedente dalla data specificata"
type: docs
weight: 190
url: /it/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Calcola la fine della data lavorativa precedente a partire dalla data specificata.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| data | DateTime | La data per calcolare la fine della giornata lavorativa precedente. |

### Valore di ritorno

La fine della giornata lavorativa precedente

## Esempi

Mostra come ottenere la fine del giorno lavorativo precedente usando un calendario.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni la fine del giorno lavorativo precedente
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// Il 9 aprile 2020 18:00 verrà stampato
Console.WriteLine(previousWorkingDayEnd);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


