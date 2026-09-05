---
title: "PrimaveraReadOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat membaca file Primavera Xml atau Primavera Xer."
type: docs
weight: 206
url: /id/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Memungkinkan untuk menentukan opsi tambahan saat membaca file Primavera Xml atau Primavera Xer.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Menginisialisasi instance baru dari kelas [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Mendapatkan flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan. |
| [getProjectUid()](#getProjectUid--) | Mendapatkan UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Mendapatkan flag yang menentukan apakah proyek baseline harus dimuat. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Mengatur flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan. |
| [setProjectUid(int value)](#setProjectUid-int-) | Mengatur UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Mengatur flag yang menentukan apakah proyek baseline harus dimuat. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Menginisialisasi instance baru dari kelas [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Mendapatkan flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan.

**Returns:**
boolean - flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Mendapatkan UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek.

**Returns:**
int - UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Mendapatkan flag yang menentukan apakah proyek baseline harus dimuat. Nilai default adalah true.

--------------------

Flag ini berlaku untuk file Primavera XML yang berisi proyek baseline (baseline tidak didukung oleh format XER). Opsi ini dapat diatur ke false untuk mempercepat pemuatan proyek besar dengan baseline ketika data baseline tidak diperlukan.

**Returns:**
boolean - flag yang menentukan apakah proyek baseline harus dimuat.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER.

**Returns:**
int - perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Mengatur flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | flag yang menentukan apakah pengidentifikasi unik asli dari entitas harus dipertahankan. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Mengatur UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | UID dari proyek yang akan dibaca dari file yang berisi beberapa proyek. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Mengatur flag yang menentukan apakah proyek baseline harus dimuat. Nilai default adalah true.

--------------------

Flag ini berlaku untuk file Primavera XML yang berisi proyek baseline (baseline tidak didukung oleh format XER). Opsi ini dapat diatur ke false untuk mempercepat pemuatan proyek besar dengan baseline ketika data baseline tidak diperlukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | flag yang menentukan apakah proyek baseline harus dimuat. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Menentukan perilaku yang digunakan untuk memproses tugas dengan kendala yang tidak terdefinisi yang dibaca dari format XER.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | perilaku yang digunakan untuk memproses tugas dengan batasan yang tidak terdefinisi yang dibaca dari format XER. |

