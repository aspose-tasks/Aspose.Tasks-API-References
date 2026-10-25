---
title: "FieldHelper"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas pembantu yang menyediakan operasi berguna dengan bidang."
type: docs
weight: 88
url: /id/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Kelas pembantu yang menyediakan operasi berguna dengan bidang.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Mengembalikan judul default dari bidang tertentu. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Mengembalikan judul default dari bidang tugas tertentu. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Mengembalikan judul default dari bidang tertentu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| field | int | Bidang untuk mendapatkan judul default. |

**Returns:**
java.lang.String - Judul default dari bidang tertentu jika bidang tersebut dapat ditampilkan dalam tampilan MS Project, null jika tidak.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Mengembalikan judul default dari bidang tugas tertentu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskKey | byte | Bidang tugas untuk mendapatkan judul default. |

**Returns:**
java.lang.String - Judul default dari bidang tugas tertentu jika bidang tersebut dapat ditampilkan dalam tampilan MS Project, null jika tidak.
