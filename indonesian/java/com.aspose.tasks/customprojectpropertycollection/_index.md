---
title: "CustomProjectPropertyCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili kumpulan properti proyek khusus."
type: docs
weight: 61
url: /id/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Mewakili kumpulan properti proyek khusus.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Menginisialisasi instance baru dari kelas [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Membuat properti khusus baru. |
| [add(String name, double value)](#add-java.lang.String-double-) | Membuat properti khusus baru. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Membuat properti khusus baru. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Membuat properti khusus baru. |
| [clear()](#clear--) | Mengosongkan PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [remove(String name)](#remove-java.lang.String-) | Menghapus properti dengan nama yang ditentukan dari koleksi. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Menginisialisasi instance baru dari kelas [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Membuat properti khusus baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama properti. |
| nilai | boolean | Nilai objek properti yang baru dibuat. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Membuat properti khusus baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama properti. |
| nilai | double | Nilai objek properti yang baru dibuat. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Membuat properti khusus baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama properti. |
| nilai | java.lang.String | Nilai objek properti yang baru dibuat. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Membuat properti khusus baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama properti. |
| nilai | java.util.Date | Nilai objek properti yang baru dibuat. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Mengosongkan PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.

**Returns:**
boolean - nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Menghapus properti dengan nama yang ditentukan dari koleksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama properti yang tidak sensitif huruf besar/kecil. |

**Returns:**
boolean - True jika elemen berhasil ditemukan dan dihapus; jika tidak, false.
