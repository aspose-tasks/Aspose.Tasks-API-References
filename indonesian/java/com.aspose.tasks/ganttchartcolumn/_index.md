---
title: "GanttChartColumn"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas tampilan Projects."
type: docs
weight: 111
url: /id/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Kelas tampilan proyek
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Menginisialisasi instance baru dari kelas GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Menginisialisasi instance baru dari kelas GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Menginisialisasi instance baru dari kelas GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Menginisialisasi instance baru dari kelas GanttChartColumn. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Mengonversi tugas saat ini menjadi teks kolom. |
| [getField()](#getField--) | Mengembalikan bidang kolom. |
| [setField(int value)](#setField-int-) | Mengatur bidang kolom. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Menginisialisasi instance baru dari kelas GanttChartColumn.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Pengonversi data tugas ke teks kolom. |
| field | int | Kolom field. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Menginisialisasi instance baru dari kelas GanttChartColumn.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Pengonversi data tugas ke teks kolom. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Menginisialisasi instance baru dari kelas GanttChartColumn.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| width | int | Lebar kolom dalam piksel. |
| field | int | Kolom field. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Menginisialisasi instance baru dari kelas GanttChartColumn.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| field | int | Kolom field. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Mengonversi tugas saat ini menjadi teks kolom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tugas saat ini. |

**Returns:**
java.lang.String - Teks kolom.
### getField() {#getField--}
```
public int getField()
```


Mengembalikan bidang kolom. `Field`.

**Returns:**
int - nilai bidang kolom.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Mengatur bidang kolom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai bidang kolom. |

