---
title: "Calendar.GetWorkingTimes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Restituisce WorkingTimeCollection dei periodi di lavoro per la data specificata"
type: docs
weight: 240
url: /it/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Restituisce [`WorkingTimeCollection`](../../workingtimecollection/) dei periodi lavorativi per la data specificata.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | DateTime | La data per cui ottenere gli orari di lavoro. |

### Valore di ritorno

Collezione di istanze di [`WorkingTime`](../../workingtime/).

## Esempi

Mostra come ottenere i periodi di lavoro per una data specifica.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni i periodi di lavoro per una data specifica
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// Verranno stampate 16 ore
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Vedi anche

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


