---
title: "AssignmentViewColumn"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas tampilan proyek."
type: docs
weight: 19
url: /id/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Kelas tampilan proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Menginisialisasi sebuah instance baru dari kelas AssignmentViewColumn. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Mengonversi penugasan sumber daya saat ini menjadi teks kolom. |
| [getField()](#getField--) | Mengembalikan bidang kolom. |
| [setField(int value)](#setField-int-) | Mengatur bidang kolom. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Menginisialisasi sebuah instance baru dari kelas AssignmentViewColumn.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Pengonversi data penugasan menjadi teks kolom. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Mengonversi penugasan sumber daya saat ini menjadi teks kolom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Penugasan saat ini. |

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

