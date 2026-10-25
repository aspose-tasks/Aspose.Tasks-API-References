---
title: "GanttBarStyle"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili gaya batang yang digunakan oleh MSP dalam tampilan Diagram Gantt."
type: docs
weight: 109
url: /id/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Mewakili gaya batang yang digunakan oleh MSP dalam tampilan Diagram Gantt.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | Menginisialisasi instansi baru dari kelas [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian bawah batang tugas. |
| [getBottomField()](#getBottomField--) | Mendapatkan data yang akan ditampilkan di bagian bawah batang. |
| [getEndShape()](#getEndShape--) | Mendapatkan bentuk akhir dari batang. |
| [getEndShapeColor()](#getEndShapeColor--) | Mendapatkan warna dari bentuk akhir. |
| [getEndShapeType()](#getEndShapeType--) | Mendapatkan tipe dari bentuk akhir. |
| [getFrom()](#getFrom--) | Mendapatkan posisi titik awal dari batang gantt. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di dalam batang tugas. |
| [getInsideField()](#getInsideField--) | Mendapatkan data yang akan ditampilkan di dalam batang. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di sebelah kiri batang tugas. |
| [getLeftField()](#getLeftField--) | Mendapatkan data yang akan ditampilkan di sebelah kiri batang. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Mendapatkan pola isi dari batang gantt. |
| [getMiddleShape()](#getMiddleShape--) | Mendapatkan bentuk tengah dari batang. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Mendapatkan warna bentuk tengah. |
| [getName()](#getName--) | Mendapatkan nama gaya. |
| [getParentStyle()](#getParentStyle--) | Mendapatkan gaya induk (atau umum) untuk gaya khusus tugas tertentu. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Mendapatkan konverter yang ditentukan pengguna untuk memperoleh teks yang ditampilkan di sebelah kanan batang tugas. |
| [getRightField()](#getRightField--) | Mendapatkan data yang akan ditampilkan di sebelah kanan batang. |
| [getRow()](#getRow--) | Mendapatkan nomor baris. |
| [getShowForCategories()](#getShowForCategories--) | Mendapatkan kategori tugas yang gaya diterapkan. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Mendapatkan Id Unik tugas yang gaya diterapkan. |
| [getStartShape()](#getStartShape--) | Mendapatkan bentuk awal batang. |
| [getStartShapeColor()](#getStartShapeColor--) | Mendapatkan warna bentuk awal. |
| [getStartShapeType()](#getStartShapeType--) | Mendapatkan tipe bentuk awal. |
| [getTo()](#getTo--) | Mendapatkan posisi titik akhir batang gantt. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Mendapatkan konverter yang ditentukan pengguna untuk memperoleh teks yang ditampilkan di bagian atas batang tugas. |
| [getTopField()](#getTopField--) | Mendapatkan data yang akan ditampilkan di bagian atas batang. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Mengatur konverter yang ditentukan pengguna untuk memperoleh teks yang ditampilkan di bagian bawah batang tugas. |
| [setBottomField(int value)](#setBottomField-int-) | Mengatur data yang akan ditampilkan di bagian bawah batang. |
| [setEndShape(int value)](#setEndShape-int-) | Mengatur bentuk akhir batang. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Mengatur warna bentuk akhir. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Mengatur tipe bentuk akhir. |
| [setFrom(int value)](#setFrom-int-) | Mengatur posisi titik awal batang gantt. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Mengatur konverter yang ditentukan pengguna untuk memperoleh teks yang ditampilkan di dalam batang tugas. |
| [setInsideField(int value)](#setInsideField-int-) | Mengatur data yang akan ditampilkan di dalam batang. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Mengatur konverter yang ditentukan pengguna untuk memperoleh teks yang ditampilkan di sebelah kiri batang tugas. |
| [setLeftField(int value)](#setLeftField-int-) | Mengatur data yang akan ditampilkan di sebelah kiri batang. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Mengatur pola isi batang gantt. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Mengatur bentuk tengah dari batang. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Mengatur warna bentuk tengah. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nama gaya. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Mengatur gaya induk (atau umum) untuk gaya khusus yang spesifik tugas. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan ditampilkan di sebelah kanan batang tugas. |
| [setRightField(int value)](#setRightField-int-) | Mengatur data yang akan ditampilkan di sebelah kanan batang. |
| [setRow(int value)](#setRow-int-) | Mengatur nomor baris. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Mengatur kategori tugas yang gaya diterapkan. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Mengatur Id Unik dari tugas yang gaya diterapkan. |
| [setStartShape(int value)](#setStartShape-int-) | Mengatur bentuk awal batang. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Mengatur warna bentuk awal. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Mengatur tipe bentuk awal. |
| [setTo(int value)](#setTo-int-) | Mengatur posisi titik akhir batang gantt. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian atas batang tugas. |
| [setTopField(int value)](#setTopField-int-) | Mengatur data yang akan ditampilkan di bagian atas batang. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


Menginisialisasi instansi baru dari kelas [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Mendapatkan konverter buatan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian bawah batang tugas. Menimpa nilai properti `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Mendapatkan data yang akan ditampilkan di bagian bawah batang. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data yang akan ditampilkan di bagian bawah batang.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Mendapatkan bentuk akhir dari batang.

**Returns:**
int - bentuk akhir batang.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Mendapatkan warna dari bentuk akhir.

**Returns:**
java.awt.Color - warna bentuk akhir.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Mendapatkan tipe bentuk akhir. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - tipe bentuk akhir.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Mendapatkan posisi titik awal batang gantt. [Field](../../com.aspose.tasks/field).

**Returns:**
int - posisi titik awal batang gantt.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan dirender di dalam batang tugas. Menimpa nilai `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) properti.

--------------------

Tidak disimpan ke format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Mendapatkan data yang akan ditampilkan di dalam batang. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data yang akan ditampilkan di dalam batang.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan dirender di sebelah kiri batang tugas. Menimpa nilai `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) properti.

--------------------

Tidak disimpan ke format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Mendapatkan data yang akan ditampilkan di sebelah kiri batang. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data yang akan ditampilkan di sebelah kiri batang.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Mendapatkan pola isi dari batang gantt.

**Returns:**
int - pola isi dari batang gantt.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Mendapatkan bentuk tengah dari batang.

**Returns:**
int - bentuk tengah batang.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Mendapatkan warna bentuk tengah.

**Returns:**
java.awt.Color - warna dari bentuk tengah.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama gaya.

**Returns:**
java.lang.String - nama gaya.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Mendapatkan gaya induk (atau umum) untuk gaya khusus tugas tertentu.

--------------------

Tugas dapat memiliki beberapa gaya khusus dengan gaya induk yang berbeda. Misalnya, pertimbangkan tugas yang memiliki gaya khusus dengan gaya induk \"Critical\" dan gaya lain dengan gaya induk \"Normal\". Singkatnya, jika tugas bersifat kritis, gaya pertama diterapkan. Jika tugas menjadi tidak kritis, gaya kedua diterapkan (logika ini diwarisi dari Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan dirender di sebelah kanan batang tugas. Menimpa nilai `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) properti.

--------------------

Tidak disimpan ke format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Mendapatkan data yang akan ditampilkan di sebelah kanan batang. [Field](../../com.aspose.tasks/field).

**Returns:**
int - data yang akan ditampilkan di sebelah kanan batang.
### getRow() {#getRow--}
```
public final int getRow()
```


Mendapatkan nomor baris.

--------------------

Bisa dari 1 hingga 4 (1 adalah nilai default).

**Returns:**
int - nomor baris.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Mendapatkan kategori tugas untuk mana gaya diterapkan. Berlaku untuk gaya induk (atau umum) batang dalam diagram Gantt (lihat `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - kategori tugas untuk mana gaya diterapkan.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Mendapatkan Id Unik dari tugas yang gaya diterapkan. Berlaku untuk gaya batang khusus tugas dalam diagram Gantt (lihat `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - Id Unik dari tugas yang gaya diterapkan.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Mendapatkan bentuk awal batang.

**Returns:**
int - bentuk awal batang.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Mendapatkan warna bentuk awal.

**Returns:**
java.awt.Color - warna dari bentuk awal.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Mendapatkan tipe bentuk awal.

**Returns:**
int - tipe bentuk awal.
### getTo() {#getTo--}
```
public final int getTo()
```


Mendapatkan posisi titik akhir batang gantt.

**Returns:**
int - posisi titik akhir batang gantt.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Mendapatkan konverter yang ditentukan pengguna untuk mendapatkan teks yang akan dirender di bagian atas batang tugas. Menimpa nilai `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) properti.

--------------------

Tidak disimpan ke format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Mendapatkan data yang akan ditampilkan di bagian atas batang.

**Returns:**
int - data yang akan ditampilkan di bagian atas batang.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan dirender di bagian bawah batang tugas. Menimpa nilai properti `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | konverter buatan pengguna untuk mendapatkan teks yang akan dirender di bagian bawah batang tugas. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Mengatur data yang akan ditampilkan di bagian bawah batang. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | data yang akan ditampilkan di bagian bawah batang. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Mengatur bentuk akhir batang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sebuah bentuk akhir batang. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Mengatur warna bentuk akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna dari bentuk akhir. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Mengatur tipe bentuk akhir. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe bentuk akhir. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Mengatur posisi titik awal batang gantt. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | posisi titik awal batang gantt. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan dirender di dalam batang tugas. Menimpa nilai properti `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | konverter buatan pengguna untuk mendapatkan teks yang akan dirender di dalam batang tugas. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Mengatur data yang akan ditampilkan di dalam batang. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | data yang akan ditampilkan di dalam batang. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan dirender di sebelah kiri batang tugas. Menimpa nilai properti `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | konverter buatan pengguna untuk mendapatkan teks yang akan dirender di sebelah kiri batang tugas. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Mengatur data yang akan ditampilkan di sebelah kiri batang. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | data yang akan ditampilkan di sebelah kiri batang. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Mengatur pola isi batang gantt.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pola isi batang gantt. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Mengatur bentuk tengah dari batang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bentuk tengah batang. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Mengatur warna bentuk tengah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna dari bentuk tengah. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Mengatur nama gaya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama gaya. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Mengatur gaya induk (atau umum) untuk gaya khusus yang spesifik tugas.

--------------------

Tugas dapat memiliki beberapa gaya khusus dengan gaya induk yang berbeda. Misalnya, pertimbangkan tugas yang memiliki gaya khusus dengan gaya induk \"Critical\" dan gaya lain dengan gaya induk \"Normal\". Singkatnya, jika tugas bersifat kritis, gaya pertama diterapkan. Jika tugas menjadi tidak kritis, gaya kedua diterapkan (logika ini diwarisi dari Microsoft Project Professional).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | gaya induk (atau umum) untuk gaya khusus yang spesifik pada tugas. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Mengatur konverter buatan pengguna untuk mendapatkan teks yang akan dirender di sebelah kanan batang tugas. Menimpa nilai properti `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di sebelah kanan batang tugas. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Mengatur data yang akan ditampilkan di sebelah kanan batang. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | data yang akan ditampilkan di sebelah kanan batang. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Mengatur nomor baris.

--------------------

Bisa dari 1 hingga 4 (1 adalah nilai default).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nomor baris. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Mengatur kategori tugas yang akan diterapkan gaya. Berlaku untuk gaya batang induk (atau umum) dalam diagram Gantt (lihat `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.List&lt;java.lang.Integer&gt; | kategori tugas yang akan diterapkan gaya. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Mengatur Id Unik dari tugas yang akan diterapkan gaya. Berlaku untuk gaya batang khusus tugas dalam diagram Gantt (lihat `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Integer | Id Unik dari tugas yang akan diterapkan gaya. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Mengatur bentuk awal batang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bentuk awal batang. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Mengatur warna bentuk awal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna dari bentuk awal. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Mengatur tipe bentuk awal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe dari bentuk awal. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Mengatur posisi titik akhir batang gantt.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | posisi titik akhir batang gantt. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Mengatur konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian atas batang tugas. Menimpa nilai properti `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)).

--------------------

Tidak disimpan ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian atas batang tugas. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Mengatur data yang akan ditampilkan di bagian atas batang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | data yang akan ditampilkan di bagian atas batang. |

