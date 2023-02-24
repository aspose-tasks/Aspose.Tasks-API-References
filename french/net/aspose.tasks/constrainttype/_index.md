---
title: Enum ConstraintType
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.ConstraintType énumération. Spécifie la contrainte sur la date de début ou de fin dune tâche.
type: docs
weight: 330
url: /fr/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Spécifie la contrainte sur la date de début ou de fin d'une tâche.

```csharp
public enum ConstraintType
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| Undefined | `-1` | La valeur n'a pas été définie dans le fichier de projet d'origine. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) et[`Finish`](../tsk/finish/) date de[`Task`](../task/) sont programmés ASAP par rapport au parent[`Start`](../tsk/start/) et[`Finish`](../tsk/finish/)dates et considérant[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) et[`Finish`](../tsk/finish/) date de[`Task`](../task/) sont programmés ALAP par rapport au parent[`Start`](../tsk/start/) et[`Finish`](../tsk/finish/)dates et considérant[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | Doit commencer le |
| MustFinishOn | `3` | Doit terminer le |
| StartNoEarlierThan | `4` | Commencer Au Plus Tôt Le |
| StartNoLaterThan | `5` | Commencer au plus tard le |
| FinishNoEarlierThan | `6` | Terminer Au Plus Tôt Le |
| FinishNoLaterThan | `7` | terminer au plus tard le |

### Remarques

Lors de l'exportation en XML, les valeurs non définies seront éliminées du XML résultant.

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


