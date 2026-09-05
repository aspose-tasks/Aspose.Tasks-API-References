---
title: "ConstraintType"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menentukan batasan pada tanggal mulai atau selesai suatu tugas."
type: docs
weight: 52
url: /id/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Menentukan batasan pada tanggal mulai atau selesai sebuah tugas. Saat mengekspor ke XML, nilai Undefined akan dihilangkan dari XML yang dihasilkan.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` dan tanggal `Tsk.Finish` dari `Task` dijadwalkan ALAP relatif terhadap tanggal `Tsk.Start` dan `Tsk.Finish` induk serta mempertimbangkan `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` dan tanggal `Tsk.Finish` dari `Task` dijadwalkan ASAP relatif terhadap tanggal `Tsk.Start` dan `Tsk.Finish` induk serta mempertimbangkan `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Selesai Tidak Lebih Awal Dari |
| [FinishNoLaterThan](#FinishNoLaterThan) | Selesaikan Tidak Lebih Lambat Dari |
| [MustFinishOn](#MustFinishOn) | Harus Selesai Pada |
| [MustStartOn](#MustStartOn) | Harus Mulai Pada |
| [StartNoEarlierThan](#StartNoEarlierThan) | Mulai Tidak Lebih Awal Dari |
| [StartNoLaterThan](#StartNoLaterThan) | Mulai Tidak Lebih Lambat Dari |
| [Undefined](#Undefined) | Nilai tidak didefinisikan dalam file proyek asli. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` dan tanggal `Tsk.Finish` dari `Task` dijadwalkan ALAP relatif terhadap tanggal `Tsk.Start` dan `Tsk.Finish` induk serta mempertimbangkan `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` dan tanggal `Tsk.Finish` dari `Task` dijadwalkan ASAP relatif terhadap tanggal `Tsk.Start` dan `Tsk.Finish` induk serta mempertimbangkan `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Selesai Tidak Lebih Awal Dari

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Selesaikan Tidak Lebih Lambat Dari

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Harus Selesai Pada

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Harus Mulai Pada

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Mulai Tidak Lebih Awal Dari

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Mulai Tidak Lebih Lambat Dari

### Undefined {#Undefined}
```
public static final int Undefined
```


Nilai tidak didefinisikan dalam file proyek asli.

