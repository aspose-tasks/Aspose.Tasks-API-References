---
title: "ResourceViewColumn"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas tampilan proyek yang digunakan dalam tampilan ResourceUsage dan tampilan ResourceSheet."
type: docs
weight: 261
url: /id/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Kelas tampilan proyek yang digunakan dalam tampilan ResourceUsage dan tampilan ResourceSheet.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Mengonversi sumber daya saat ini menjadi teks kolom. |
| [getField()](#getField--) | Mengembalikan bidang kolom. |
| [setField(int value)](#setField-int-) | Mengatur bidang kolom. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Pengonversi data sumber daya ke teks kolom. |
| field | int | Kolom field. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama kolom. |
| width | int | Lebar kolom dalam piksel. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Pengonversi data sumber daya ke teks kolom. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Menginisialisasi instance baru dari kelas [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| width | int | Lebar kolom dalam piksel. |
| field | int | Kolom field. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Mengonversi sumber daya saat ini menjadi teks kolom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Sumber daya saat ini. |

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

