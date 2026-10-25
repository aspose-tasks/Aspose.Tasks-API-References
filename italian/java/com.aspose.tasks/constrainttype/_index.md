---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API Reference"
description: "Specifica il vincolo sulla data di inizio o di fine di un'attività."
type: docs
weight: 52
url: /it/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Specifica il vincolo sulla data di inizio o di fine di un'attività. Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.
## Campi

| Campo | Descrizione |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` e le date `Tsk.Finish` di `Task` sono programmate ALAP rispetto alle date `Tsk.Start` e `Tsk.Finish` del genitore e considerando `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` e le date `Tsk.Finish` di `Task` sono programmate ASAP rispetto alle date `Tsk.Start` e `Tsk.Finish` del genitore e considerando `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Fine non prima di |
| [FinishNoLaterThan](#FinishNoLaterThan) | Finisci non più tardi di |
| [MustFinishOn](#MustFinishOn) | Deve terminare il |
| [MustStartOn](#MustStartOn) | Deve iniziare il |
| [StartNoEarlierThan](#StartNoEarlierThan) | Inizia non prima di |
| [StartNoLaterThan](#StartNoLaterThan) | Inizia non più tardi di |
| [Undefined](#Undefined) | Il valore non era definito nel file di progetto originale. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` e le date `Tsk.Finish` di `Task` sono programmate ALAP rispetto alle date `Tsk.Start` e `Tsk.Finish` del genitore e considerando `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` e le date `Tsk.Finish` di `Task` sono programmate ASAP rispetto alle date `Tsk.Start` e `Tsk.Finish` del genitore e considerando `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Fine non prima di

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Finisci non più tardi di

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Deve terminare il

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Deve iniziare il

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Inizia non prima di

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Inizia non più tardi di

### Undefined {#Undefined}
```
public static final int Undefined
```


Il valore non era definito nel file di progetto originale.

