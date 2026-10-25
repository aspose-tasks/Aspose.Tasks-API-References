---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API-referens"
description: "Anger begränsningen för start- eller slutdatum för en uppgift."
type: docs
weight: 52
url: /sv/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Anger begränsningen för start- eller slutdatum för en uppgift. Vid export till XML kommer odefinierade värden att tas bort från den resulterande XML‑filen.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` och `Tsk.Finish` datum för `Task` schemaläggs ALAP i förhållande till förälderns `Tsk.Start` och `Tsk.Finish` datum och med beaktande av `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` och `Tsk.Finish` datum för `Task` schemaläggs ASAP i förhållande till förälderns `Tsk.Start` och `Tsk.Finish` datum och med beaktande av `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Slut inte tidigare än |
| [FinishNoLaterThan](#FinishNoLaterThan) | Slut inte senare än |
| [MustFinishOn](#MustFinishOn) | Måste sluta på |
| [MustStartOn](#MustStartOn) | Måste starta på |
| [StartNoEarlierThan](#StartNoEarlierThan) | Start inte tidigare än |
| [StartNoLaterThan](#StartNoLaterThan) | Start inte senare än |
| [Undefined](#Undefined) | Värdet var inte definierat i den ursprungliga projektfilen. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` och `Tsk.Finish` datum för `Task` schemaläggs ALAP i förhållande till förälderns `Tsk.Start` och `Tsk.Finish` datum och med beaktande av `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` och `Tsk.Finish` datum för `Task` schemaläggs ASAP i förhållande till förälderns `Tsk.Start` och `Tsk.Finish` datum och med beaktande av `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Slut inte tidigare än

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Slut inte senare än

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Måste sluta på

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Måste starta på

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Start inte tidigare än

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Start inte senare än

### Undefined {#Undefined}
```
public static final int Undefined
```


Värdet var inte definierat i den ursprungliga projektfilen.

