---
title: Enum ConstraintType
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.ConstraintType enum. Specifica il vincolo sulla data di inizio o fine di unattività.
type: docs
weight: 330
url: /it/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Specifica il vincolo sulla data di inizio o fine di un'attività.

```csharp
public enum ConstraintType
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il valore non è stato definito nel file di progetto originale. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) E[`Finish`](../tsk/finish/) date di[`Task`](../task/) sono programmati ASAP rispetto al genitore[`Start`](../tsk/start/) E[`Finish`](../tsk/finish/)date e considerando[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) E[`Finish`](../tsk/finish/) date di[`Task`](../task/) sono programmati ALAP rispetto al genitore[`Start`](../tsk/start/) E[`Finish`](../tsk/finish/)date e considerando[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | Deve iniziare il |
| MustFinishOn | `3` | Deve finire il |
| StartNoEarlierThan | `4` | Inizia non prima del |
| StartNoLaterThan | `5` | Inizia non più tardi di |
| FinishNoEarlierThan | `6` | Termina non prima del |
| FinishNoLaterThan | `7` | Termina non più tardi di |

### Osservazioni

Durante l'esportazione in XML i valori non definiti verranno eliminati dall'XML risultante.

### Guarda anche

* spazio dei nomi [Aspose.Tasks](../../aspose.tasks/)
* assemblea [Aspose.Tasks](../../)


