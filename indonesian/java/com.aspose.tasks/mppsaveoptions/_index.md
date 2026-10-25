---
title: "MPPSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat menyimpan data proyek ke MPP."
type: docs
weight: 149
url: /id/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat menyimpan data proyek ke MPP.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Menginisialisasi instance baru dari kelas [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getClearVba()](#getClearVba--) | Mendapatkan nilai yang menunjukkan apakah data makro VBA yang ada harus dihapus saat menyimpan proyek ke format MPP. |
| [getProtectionPassword()](#getProtectionPassword--) | Mendapatkan kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya yang tidak valid harus dihapus saat menyimpan ke MPP. |
| [getWriteFilters()](#getWriteFilters--) | Mendapatkan nilai yang menunjukkan apakah data filter harus ditulis saat menyimpan proyek ke format MPP. |
| [getWriteGroups()](#getWriteGroups--) | Mendapatkan nilai yang menunjukkan apakah menulis data grup saat menyimpan proyek ke MPP untuk format. |
| [getWriteVba()](#getWriteVba--) | Mendapatkan nilai yang menunjukkan apakah memperbarui data makro VBA yang ada dalam file MPP. |
| [getWriteViewData()](#getWriteViewData--) | Mendapatkan nilai yang menunjukkan apakah menulis data tampilan saat menyimpan proyek ke format MPP. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Mengatur nilai yang menunjukkan apakah menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Mengatur kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Mengatur nilai yang menunjukkan apakah menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Mengatur nilai yang menunjukkan apakah menulis data filter saat menyimpan proyek ke MPP untuk format. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Mengatur nilai yang menunjukkan apakah menulis data grup saat menyimpan proyek ke MPP untuk format. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Mengatur nilai yang menunjukkan apakah memperbarui data makro VBA yang ada dalam file MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Mengatur nilai yang menunjukkan apakah menulis data tampilan saat menyimpan proyek ke format MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Menginisialisasi instance baru dari kelas [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Mendapatkan nilai yang menunjukkan apakah data makro VBA yang ada harus dihapus saat menyimpan proyek ke format MPP.

**Returns:**
boolean - nilai yang menunjukkan apakah menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Mendapatkan kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. Saat ini didukung untuk MS Project 2010 dan format yang lebih baru.

--------------------

Nilai null menunjukkan bahwa file proyek tidak dilindungi.

**Returns:**
java.lang.String - kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya yang tidak valid harus dihapus saat menyimpan ke MPP.

--------------------

MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Atur flag ini ke true untuk menghapusnya saat menyimpan.

**Returns:**
boolean - nilai yang menunjukkan apakah menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Mendapatkan nilai yang menunjukkan apakah data filter harus ditulis saat menyimpan proyek ke format MPP.

--------------------

Data filter mencakup koleksi Project.TaskFilters dan Project.ResourceFilters.

--------------------

Saat ini didukung untuk MSP 2010 atau format yang lebih baru.

**Returns:**
boolean - nilai yang menunjukkan apakah menulis data filter saat menyimpan proyek ke MPP untuk format.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Mendapatkan nilai yang menunjukkan apakah menulis data grup saat menyimpan proyek ke MPP untuk format.

--------------------

Data grup mencakup koleksi Project.TaskGroups dan Project.ResourceGroups.

**Returns:**
boolean - nilai yang menunjukkan apakah menulis data grup saat menyimpan proyek ke MPP untuk format.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Mendapatkan nilai yang menunjukkan apakah memperbarui data makro VBA yang ada dalam file MPP. Saat ini penulisan VbaModule.SourceCode didukung.

**Returns:**
boolean - nilai yang menunjukkan apakah memperbarui data makro VBA yang ada dalam file MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Mendapatkan nilai yang menunjukkan apakah menulis data tampilan saat menyimpan proyek ke format MPP.

--------------------

Data tampilan mencakup koleksi Project.Views, Filters, dan Tables.

**Returns:**
boolean - nilai yang menunjukkan apakah menulis data tampilan saat menyimpan proyek ke format MPP.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Mengatur nilai yang menunjukkan apakah menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Mengatur kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. Saat ini didukung untuk format MS Project 2010 dan yang lebih baru.

--------------------

Nilai null menunjukkan bahwa file proyek tidak dilindungi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi yang digunakan untuk melindungi file MPP yang dihasilkan. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Mengatur nilai yang menunjukkan apakah menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP.

--------------------

MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Atur flag ini ke true untuk menghapusnya saat menyimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Mengatur nilai yang menunjukkan apakah menulis data filter saat menyimpan proyek ke MPP untuk format.

--------------------

Data filter mencakup koleksi Project.TaskFilters dan Project.ResourceFilters.

--------------------

Saat ini didukung untuk MSP 2010 atau format yang lebih baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menulis data filter saat menyimpan proyek ke format MPP. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Mengatur nilai yang menunjukkan apakah menulis data grup saat menyimpan proyek ke MPP untuk format.

--------------------

Data grup mencakup koleksi Project.TaskGroups dan Project.ResourceGroups.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menulis data grup saat menyimpan proyek ke format MPP. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan memperbarui data makro VBA yang ada dalam file MPP. Saat ini penulisan VbaModule.SourceCode didukung.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan memperbarui data makro VBA yang ada dalam file MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Mengatur nilai yang menunjukkan apakah menulis data tampilan saat menyimpan proyek ke format MPP.

--------------------

Data tampilan mencakup koleksi Project.Views, Filters, dan Tables.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menulis data tampilan saat menyimpan proyek ke format MPP. |

