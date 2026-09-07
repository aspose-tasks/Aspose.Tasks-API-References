---
title: "Enum TaskStatus"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.TaskStatus enum. Specifica lo stato di un'attività"
type: docs
weight: 2460
url: /it/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

Specifica lo stato di un'attività.

```csharp
public enum TaskStatus
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Stato dell'attività non definito. |
| Complete | `0` | L'attività è completata al 100 percento. |
| OnSchedule | `1` | L'attività è in programma se timephased cumulative percent complete è distribuita almeno fino al giorno precedente la data di stato. |
| Late | `2` | L'attività è in ritardo se timephased cumulative percent complete non raggiunge la mezzanotte del giorno precedente la data di stato. |
| Future | `3` | Lo stato dell'attività 'Future' viene impostato quando la data di inizio dell'attività è successiva alla data di stato. |

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


