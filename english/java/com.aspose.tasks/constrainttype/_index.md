---
title: ConstraintType
second_title: Aspose.Tasks for Java API Reference
description: Specifies the constraint on the start or finish date of a task.
type: docs
weight: 52
url: /java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Specifies the constraint on the start or finish date of a task. While exporting into XML the Undefined values will be eliminated from resulting XML.
## Fields

| Field | Description |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` and `Tsk.Finish` dates of `Task` are scheduled ALAP with respect to parent `Tsk.Start` and `Tsk.Finish` dates and considering `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` and `Tsk.Finish` dates of `Task` are scheduled ASAP with respect to parent `Tsk.Start` and `Tsk.Finish` dates and considering `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Finish No Earlier Than |
| [FinishNoLaterThan](#FinishNoLaterThan) | Finish No Later Than |
| [MustFinishOn](#MustFinishOn) | Must Finish On |
| [MustStartOn](#MustStartOn) | Must Start On |
| [StartNoEarlierThan](#StartNoEarlierThan) | Start No Earlier Than |
| [StartNoLaterThan](#StartNoLaterThan) | Start No Later Than |
| [Undefined](#Undefined) | The value was not defined in original project file. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` and `Tsk.Finish` dates of `Task` are scheduled ALAP with respect to parent `Tsk.Start` and `Tsk.Finish` dates and considering `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` and `Tsk.Finish` dates of `Task` are scheduled ASAP with respect to parent `Tsk.Start` and `Tsk.Finish` dates and considering `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Finish No Earlier Than

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Finish No Later Than

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Must Finish On

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Must Start On

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Start No Earlier Than

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Start No Later Than

### Undefined {#Undefined}
```
public static final int Undefined
```


The value was not defined in original project file.

