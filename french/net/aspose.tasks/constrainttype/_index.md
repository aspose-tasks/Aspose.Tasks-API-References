---
title: "Énum ConstraintType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énum Aspose.Tasks.ConstraintType. Spécifie la contrainte sur la date de début ou de fin d'une tâche"
type: docs
weight: 330
url: /fr/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Spécifie la contrainte sur la date de début ou de fin d’une tâche.

```csharp
public enum ConstraintType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | La valeur n'était pas définie dans le fichier de projet original. |
| AsSoonAsPossible | `0` | Les dates de [`Start`](../tsk/start/) et de [`Finish`](../tsk/finish/) de la [`Task`](../task/) sont planifiées dès que possible par rapport aux dates parent [`Start`](../tsk/start/) et [`Finish`](../tsk/finish/) et en tenant compte des [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) et les dates de [`Finish`](../tsk/finish/) de la [`Task`](../task/) sont planifiées ALAP par rapport aux dates parent [`Start`](../tsk/start/) et [`Finish`](../tsk/finish/) et en tenant compte des [`TaskLinks`](../project/tasklinks/).` |
| MustStartOn | `2` | Doit commencer le |
| MustFinishOn | `3` | Doit se terminer le |
| StartNoEarlierThan | `4` | Commencer pas avant le |
| StartNoLaterThan | `5` | Commencer pas après le |
| FinishNoEarlierThan | `6` | Terminer pas avant le |
| FinishNoLaterThan | `7` | Terminer pas après le |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment définir la contrainte &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible pour une tâche.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Définir la contrainte As Soon As Possible pour la tâche avec l'Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


