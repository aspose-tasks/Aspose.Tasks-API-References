---
title: "ConstraintType"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir görevin başlangıç veya bitiş tarihine ilişkin kısıtlamayı belirtir."
type: docs
weight: 52
url: /tr/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Bir görevin başlangıç veya bitiş tarihine ilişkin kısıtlamayı belirtir. XML'e dışa aktarırken Undefined değerleri sonuç XML'inden kaldırılacaktır.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Task`'in `Tsk.Start` ve `Tsk.Finish` tarihleri, üst `Tsk.Start` ve `Tsk.Finish` tarihleri ve `Project.TaskLinks` dikkate alınarak ALAP olarak planlanır. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Task`'in `Tsk.Start` ve `Tsk.Finish` tarihleri, üst `Tsk.Start` ve `Tsk.Finish` tarihleri ve `Project.TaskLinks` dikkate alınarak ASAP olarak planlanır. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Bitiş Erken Olmaz |
| [FinishNoLaterThan](#FinishNoLaterThan) | En geç bitir |
| [MustFinishOn](#MustFinishOn) | Şu tarihte bitirilmelidir |
| [MustStartOn](#MustStartOn) | Şu tarihte başlamalıdır |
| [StartNoEarlierThan](#StartNoEarlierThan) | En erken bu tarihten önce başla |
| [StartNoLaterThan](#StartNoLaterThan) | En geç bu tarihte başla |
| [Undefined](#Undefined) | Değer, orijinal proje dosyasında tanımlanmamıştı. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Task`'in `Tsk.Start` ve `Tsk.Finish` tarihleri, üst `Tsk.Start` ve `Tsk.Finish` tarihleri ve `Project.TaskLinks` dikkate alınarak ALAP olarak planlanır.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Task`'in `Tsk.Start` ve `Tsk.Finish` tarihleri, üst `Tsk.Start` ve `Tsk.Finish` tarihleri ve `Project.TaskLinks` dikkate alınarak ASAP olarak planlanır.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Bitiş Erken Olmaz

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


En geç bitir

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Şu tarihte bitirilmelidir

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Şu tarihte başlamalıdır

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


En erken bu tarihten önce başla

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


En geç bu tarihte başla

### Undefined {#Undefined}
```
public static final int Undefined
```


Değer, orijinal proje dosyasında tanımlanmamıştı.

