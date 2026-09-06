---
title: "ConstraintType"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Especifica la restricción sobre la fecha de inicio o fin de una tarea."
type: docs
weight: 52
url: /es/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Especifica la restricción en la fecha de inicio o fin de una tarea. Al exportar a XML, los valores Undefined se eliminarán del XML resultante.
## Campos

| Campo | Descripción |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` y `Tsk.Finish` fechas de `Task` se programan ALAP con respecto a las fechas padre `Tsk.Start` y `Tsk.Finish` y considerando `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` y `Tsk.Finish` fechas de `Task` se programan ASAP con respecto a las fechas padre `Tsk.Start` y `Tsk.Finish` y considerando `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Finalizar No Antes De |
| [FinishNoLaterThan](#FinishNoLaterThan) | Finalizar no más tarde que |
| [MustFinishOn](#MustFinishOn) | Debe finalizar el |
| [MustStartOn](#MustStartOn) | Debe iniciar el |
| [StartNoEarlierThan](#StartNoEarlierThan) | Iniciar no antes de |
| [StartNoLaterThan](#StartNoLaterThan) | Iniciar no más tarde que |
| [Undefined](#Undefined) | El valor no estaba definido en el archivo de proyecto original. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` y `Tsk.Finish` fechas de `Task` se programan ALAP con respecto a las fechas padre `Tsk.Start` y `Tsk.Finish` y considerando `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` y `Tsk.Finish` fechas de `Task` se programan ASAP con respecto a las fechas padre `Tsk.Start` y `Tsk.Finish` y considerando `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Finalizar No Antes De

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Finalizar no más tarde que

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Debe finalizar el

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Debe iniciar el

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Iniciar no antes de

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Iniciar no más tarde que

### Undefined {#Undefined}
```
public static final int Undefined
```


El valor no estaba definido en el archivo de proyecto original.

