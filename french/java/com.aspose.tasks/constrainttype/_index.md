---
title: "ConstraintType"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Spécifie la contrainte sur la date de début ou de fin d'une tâche."
type: docs
weight: 52
url: /fr/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Spécifie la contrainte sur la date de début ou de fin d'une tâche. Lors de l'exportation en XML, les valeurs Undefined seront éliminées du XML résultant.
## Champs

| Champ | Description |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` et `Tsk.Finish` dates de `Task` sont planifiées ALAP par rapport aux dates parent `Tsk.Start` et `Tsk.Finish` et en tenant compte de `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` et `Tsk.Finish` dates de `Task` sont planifiées ASAP par rapport aux dates parent `Tsk.Start` et `Tsk.Finish` et en tenant compte de `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Fin pas antérieure à |
| [FinishNoLaterThan](#FinishNoLaterThan) | Finir au plus tard |
| [MustFinishOn](#MustFinishOn) | Doit se terminer le |
| [MustStartOn](#MustStartOn) | Doit commencer le |
| [StartNoEarlierThan](#StartNoEarlierThan) | Commencer au plus tôt |
| [StartNoLaterThan](#StartNoLaterThan) | Commencer au plus tard |
| [Undefined](#Undefined) | La valeur n'était pas définie dans le fichier de projet original. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` et `Tsk.Finish` dates de `Task` sont planifiées ALAP par rapport aux dates parent `Tsk.Start` et `Tsk.Finish` et en tenant compte de `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` et `Tsk.Finish` dates de `Task` sont planifiées ASAP par rapport aux dates parent `Tsk.Start` et `Tsk.Finish` et en tenant compte de `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Fin pas antérieure à

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Finir au plus tard

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Doit se terminer le

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Doit commencer le

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Commencer au plus tôt

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Commencer au plus tard

### Undefined {#Undefined}
```
public static final int Undefined
```


La valeur n'était pas définie dans le fichier de projet original.

