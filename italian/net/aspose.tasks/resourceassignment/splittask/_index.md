---
title: ResourceAssignment.SplitTask
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ResourceAssignment metodo. Divide lattività in due parti.
type: docs
weight: 750
url: /it/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divide l'attività in due parti.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| start | DateTime | L'inizio dell'interruzione del lavoro da suddividere in base a. |
| finish | DateTime | La fine dell'interruzione del lavoro da suddividere in base a. |
| calendar | Calendar | Il calendario da suddividere in base a. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | Genera quando la data di inizio è precedente alla data di inizio dell'assegnazione. |
| ArgumentOutOfRangeException | Genera quando la data di fine è successiva alla data di fine dell'assegnazione. |

### Guarda anche

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* spazio dei nomi [Aspose.Tasks](../../resourceassignment/)
* assemblea [Aspose.Tasks](../../../)


