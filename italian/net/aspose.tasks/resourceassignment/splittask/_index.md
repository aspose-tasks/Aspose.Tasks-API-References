---
title: SplitTask
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Divide lattività in due parti.
type: docs
weight: 150
url: /it/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divide l'attività in due parti.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| start | DateTime | L'inizio dell'interruzione del lavoro su cui dividere. |
| finish | DateTime | La fine dell'interruzione del lavoro su cui dividere in base. |
| calendar | Calendar | Il calendario in base al quale dividere. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentOutOfRangeException | Genera quando la data di inizio è inferiore alla data di inizio dell'assegnazione. |
| ArgumentOutOfRangeException | Genera quando la data di fine è maggiore della data di fine dell'assegnazione. |

### Guarda anche

* class [Calendar](../../calendar)
* class [ResourceAssignment](../../resourceassignment)
* spazio dei nomi [Aspose.Tasks](../../resourceassignment)
* assemblea [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->