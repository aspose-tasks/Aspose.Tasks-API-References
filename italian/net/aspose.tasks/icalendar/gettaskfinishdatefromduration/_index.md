---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ICalendar. Calcola la data e l'ora di fine attività dalla sua data di inizio suddivisa e dalla durata del lavoro."
type: docs
weight: 50
url: /it/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Calcola la data e l'ora di fine dell'attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | Attività | L'attività per cui calcolare la data di fine. |
| durata | TimeSpan | La durata da calcolare. |

### Valore di ritorno

Data di fine dell'attività per la data di inizio e la durata fornite.

## Osservazioni

Restituisce DateTime.MinValue se l'attività è un riepilogo, null o se la sua data di inizio non è impostata.

### Vedi anche

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


