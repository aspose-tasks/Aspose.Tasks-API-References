---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Calendar metodo. Calcola la data e lora di fine dellattività dalla data di inizio le parti divise e la durata.
type: docs
weight: 190
url: /it/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calcola la data e l'ora di fine dell'attività dalla data di inizio, le parti divise e la durata.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | Task | L'attività per cui ottenere la data di fine. |
| duration | TimeSpan | La durata dell'attività in base alla quale suddividere. |

### Valore di ritorno

Data di fine dell'attività.

### Osservazioni

Restituisce DateTime.MinValue se l'attività è di riepilogo, null o la data di inizio non è impostata.

### Guarda anche

* class [Task](../../task/)
* class [Calendar](../)
* spazio dei nomi [Aspose.Tasks](../../calendar/)
* assemblea [Aspose.Tasks](../../../)


