---
title: "TaskStatus"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menentukan status sebuah tugas."
type: docs
weight: 301
url: /id/java/com.aspose.tasks/taskstatus/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TaskStatus extends System.Enum
```

Menentukan status sebuah tugas.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [Complete](#Complete) | Tugas selesai 100 persen. |
| [Future](#Future) | Status tugas 'Future' diatur ketika tanggal mulai tugas lebih besar dari tanggal status. |
| [Late](#Late) | Tugas terlambat jika timephased cumulative percent complete tidak mencapai tengah malam pada hari sebelum tanggal status. |
| [OnSchedule](#OnSchedule) | Tugas tepat waktu jika timephased cumulative percent complete tersebar setidaknya hingga hari sebelum tanggal status. |
| [Undefined](#Undefined) | Status tugas tidak terdefinisi. |
### Complete {#Complete}
```
public static final int Complete
```


Tugas selesai 100 persen.

### Future {#Future}
```
public static final int Future
```


Status tugas 'Future' diatur ketika tanggal mulai tugas lebih besar dari tanggal status.

### Late {#Late}
```
public static final int Late
```


Tugas terlambat jika timephased cumulative percent complete tidak mencapai tengah malam pada hari sebelum tanggal status.

### OnSchedule {#OnSchedule}
```
public static final int OnSchedule
```


Tugas tepat waktu jika timephased cumulative percent complete tersebar setidaknya hingga hari sebelum tanggal status.

### Undefined {#Undefined}
```
public static final int Undefined
```


Status tugas tidak terdefinisi.

