---
title: "TaskTextStyleEventArgs"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas ini mewakili sekumpulan data yang terkait dengan rendering konten sel tabel."
type: docs
weight: 302
url: /id/java/com.aspose.tasks/tasktextstyleeventargs/
---

**Inheritance:**
java.lang.Object
```
public class TaskTextStyleEventArgs
```

Kelas ini mewakili sekumpulan data yang terkait dengan perenderan konten sel tabel.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCellTextStyle()](#getCellTextStyle--) | Mendapatkan TextStyle yang akan digunakan untuk menggambar konten sel. |
| [getColumn()](#getColumn--) | Mendapatkan [ViewColumn](../../com.aspose.tasks/viewcolumn) yang menjadi milik sel yang sedang dirender. |
| [getTask()](#getTask--) | Mendapatkan `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) yang sesuai dengan baris yang sedang ditampilkan. |
| [setCellTextStyle(TextStyle value)](#setCellTextStyle-com.aspose.tasks.TextStyle-) | Menetapkan TextStyle yang akan digunakan untuk menggambar konten sel. |
### getCellTextStyle() {#getCellTextStyle--}
```
public final TextStyle getCellTextStyle()
```


Mendapatkan TextStyle yang akan digunakan untuk menggambar konten sel. Objek ini dapat digunakan untuk menyesuaikan tampilan sel tabel.

**Returns:**
[TextStyle](../../com.aspose.tasks/textstyle) - TextStyle which will be used to draw the cell's content.
### getColumn() {#getColumn--}
```
public final ViewColumn getColumn()
```


Mendapatkan [ViewColumn](../../com.aspose.tasks/viewcolumn) yang menjadi milik sel yang sedang dirender.

**Returns:**
[ViewColumn](../../com.aspose.tasks/viewcolumn) - [ViewColumn](../../com.aspose.tasks/viewcolumn) to which the currently rendered cell belongs.
### getTask() {#getTask--}
```
public final Task getTask()
```


Mendapatkan `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) yang sesuai dengan baris yang sedang ditampilkan.

**Returns:**
[Task](../../com.aspose.tasks/task) - `Task`([getTask()](../../com.aspose.tasks/tasktextstyleeventargs\#getTask--)/[setTask(Task)](../../com.aspose.tasks/tasktextstyleeventargs\#setTask-Task-)) which corresponds to the currently rendered row.
### setCellTextStyle(TextStyle value) {#setCellTextStyle-com.aspose.tasks.TextStyle-}
```
public final void setCellTextStyle(TextStyle value)
```


Menetapkan TextStyle yang akan digunakan untuk menggambar konten sel. Objek ini dapat digunakan untuk menyesuaikan tampilan sel tabel.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TextStyle](../../com.aspose.tasks/textstyle) | TextStyle yang akan digunakan untuk menggambar konten sel. |

