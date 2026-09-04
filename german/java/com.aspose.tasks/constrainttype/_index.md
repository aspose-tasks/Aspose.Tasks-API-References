---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gibt die Einschränkung für das Start- oder Enddatum einer Aufgabe an."
type: docs
weight: 52
url: /de/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Gibt die Einschränkung für das Start- oder Enddatum einer Aufgabe an. Beim Exportieren nach XML werden die undefinierten Werte aus dem resultierenden XML entfernt.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` und `Tsk.Finish` Daten von `Task` werden ALAP in Bezug auf die übergeordneten `Tsk.Start`- und `Tsk.Finish`-Daten geplant, wobei `Project.TaskLinks` berücksichtigt werden. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` und `Tsk.Finish` Daten von `Task` werden ASAP in Bezug auf die übergeordneten `Tsk.Start`- und `Tsk.Finish`-Daten geplant, wobei `Project.TaskLinks` berücksichtigt werden. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Ende nicht früher als |
| [FinishNoLaterThan](#FinishNoLaterThan) | Ende nicht später als |
| [MustFinishOn](#MustFinishOn) | Muss enden am |
| [MustStartOn](#MustStartOn) | Muss beginnen am |
| [StartNoEarlierThan](#StartNoEarlierThan) | Start nicht früher als |
| [StartNoLaterThan](#StartNoLaterThan) | Start nicht später als |
| [Undefined](#Undefined) | Der Wert war in der ursprünglichen Projektdatei nicht definiert. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` und `Tsk.Finish` Daten von `Task` werden ALAP in Bezug auf die übergeordneten `Tsk.Start`- und `Tsk.Finish`-Daten geplant, wobei `Project.TaskLinks` berücksichtigt werden.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` und `Tsk.Finish` Daten von `Task` werden ASAP in Bezug auf die übergeordneten `Tsk.Start`- und `Tsk.Finish`-Daten geplant, wobei `Project.TaskLinks` berücksichtigt werden.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Ende nicht früher als

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Ende nicht später als

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Muss enden am

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Muss beginnen am

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Start nicht früher als

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Start nicht später als

### Undefined {#Undefined}
```
public static final int Undefined
```


Der Wert war in der ursprünglichen Projektdatei nicht definiert.

