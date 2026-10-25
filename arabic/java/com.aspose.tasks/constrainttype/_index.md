---
title: "ConstraintType"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد القيد على تاريخ البدء أو الانتهاء للمهمة."
type: docs
weight: 52
url: /ar/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

يحدد القيد على تاريخ البدء أو الانتهاء لمهمة. أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.
## الحقول

| حقل | الوصف |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` و `Tsk.Finish` لتاريخ `Task` يتم جدولتهما وفقاً لأقرب موعد ممكن (ALAP) بالنسبة لتواريخ `Tsk.Start` و `Tsk.Finish` للأصل مع مراعاة `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` و `Tsk.Finish` لتاريخ `Task` يتم جدولتهما وفقاً لأقرب وقت ممكن (ASAP) بالنسبة لتواريخ `Tsk.Start` و `Tsk.Finish` للأصل مع مراعاة `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | الانتهاء ليس قبل |
| [FinishNoLaterThan](#FinishNoLaterThan) | الانتهاء ليس بعد |
| [MustFinishOn](#MustFinishOn) | يجب الانتهاء في |
| [MustStartOn](#MustStartOn) | يجب البدء في |
| [StartNoEarlierThan](#StartNoEarlierThan) | البدء ليس قبل |
| [StartNoLaterThan](#StartNoLaterThan) | البدء ليس بعد |
| [Undefined](#Undefined) | القيمة لم تُحدد في ملف المشروع الأصلي. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` و `Tsk.Finish` لتاريخ `Task` يتم جدولتهما وفقاً لأقرب موعد ممكن (ALAP) بالنسبة لتواريخ `Tsk.Start` و `Tsk.Finish` للأصل مع مراعاة `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` و `Tsk.Finish` لتاريخ `Task` يتم جدولتهما وفقاً لأقرب وقت ممكن (ASAP) بالنسبة لتواريخ `Tsk.Start` و `Tsk.Finish` للأصل مع مراعاة `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


الانتهاء ليس قبل

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


الانتهاء ليس بعد

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


يجب الانتهاء في

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


يجب البدء في

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


البدء ليس قبل

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


البدء ليس بعد

### Undefined {#Undefined}
```
public static final int Undefined
```


القيمة لم تُحدد في ملف المشروع الأصلي.

