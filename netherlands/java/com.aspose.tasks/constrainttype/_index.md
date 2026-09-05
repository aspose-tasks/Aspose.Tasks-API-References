---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Specificeert de beperking op de start- of einddatum van een taak."
type: docs
weight: 52
url: /nl/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Specificeert de beperking op de start- of einddatum van een taak. Bij het exporteren naar XML worden de Undefined-waarden verwijderd uit de resulterende XML.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` en `Tsk.Finish` datums van `Task` worden gepland ALAP ten opzichte van de bovenliggende `Tsk.Start` en `Tsk.Finish` datums, rekening houdend met `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` en `Tsk.Finish` datums van `Task` worden gepland ASAP ten opzichte van de bovenliggende `Tsk.Start` en `Tsk.Finish` datums, rekening houdend met `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Eind Niet Vroeger Dan |
| [FinishNoLaterThan](#FinishNoLaterThan) | Voltooi niet later dan |
| [MustFinishOn](#MustFinishOn) | Moet eindigen op |
| [MustStartOn](#MustStartOn) | Moet beginnen op |
| [StartNoEarlierThan](#StartNoEarlierThan) | Begin niet eerder dan |
| [StartNoLaterThan](#StartNoLaterThan) | Begin niet later dan |
| [Undefined](#Undefined) | De waarde was niet gedefinieerd in het oorspronkelijke projectbestand. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` en `Tsk.Finish` datums van `Task` worden gepland ALAP ten opzichte van de bovenliggende `Tsk.Start` en `Tsk.Finish` datums, rekening houdend met `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` en `Tsk.Finish` datums van `Task` worden gepland ASAP ten opzichte van de bovenliggende `Tsk.Start` en `Tsk.Finish` datums, rekening houdend met `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Eind Niet Vroeger Dan

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Voltooi niet later dan

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Moet eindigen op

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Moet beginnen op

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Begin niet eerder dan

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Begin niet later dan

### Undefined {#Undefined}
```
public static final int Undefined
```


De waarde was niet gedefinieerd in het oorspronkelijke projectbestand.

