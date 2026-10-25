---
title: "ITextStyleModificationCallback"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili callback yang dipanggil sebelum TextStyle diterapkan ke sel tabel."
type: docs
weight: 383
url: /id/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Mewakili callback yang dipanggil sebelum TextStyle diterapkan ke sel tabel.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Metode yang akan dipanggil sebelum merender sel tabel untuk baris tugas pada tampilan berikut: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Metode yang akan dipanggil sebelum merender sel tabel untuk baris tugas pada tampilan berikut: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | Objek [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

