---
title: "Enum ConstraintType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.ConstraintType. Specifica il vincolo sulla data di inizio o fine di un'attività"
type: docs
weight: 330
url: /it/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Specifica il vincolo sulla data di inizio o di fine di un'attività.

```csharp
public enum ConstraintType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il valore non era definito nel file di progetto originale. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) e le date di [`Finish`](../tsk/finish/) dell'[`Task`](../task/) sono programmate il prima possibile rispetto alle date di [`Start`](../tsk/start/) e [`Finish`](../tsk/finish/) del genitore e tenendo conto dei [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | Le date di [`Start`](../tsk/start/) e [`Finish`](../tsk/finish/) del [`Task`](../task/) sono programmate ALAP rispetto alle date di [`Start`](../tsk/start/) e [`Finish`](../tsk/finish/) del genitore e considerando i [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Deve iniziare il |
| MustFinishOn | `3` | Deve terminare il |
| StartNoEarlierThan | `4` | Inizio non prima di |
| StartNoLaterThan | `5` | Inizio non oltre |
| FinishNoEarlierThan | `6` | Fine non prima di |
| FinishNoLaterThan | `7` | Fine non oltre |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come impostare il vincolo &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible per un'attività.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Imposta il vincolo As Soon As Possible per l'attività con Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


