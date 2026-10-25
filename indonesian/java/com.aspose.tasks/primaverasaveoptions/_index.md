---
title: "PrimaveraSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera XER."
type: docs
weight: 208
url: /id/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera XER.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Menginisialisasi instance baru dari kelas [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Mendapatkan kenaikan yang digunakan dalam penomoran ulang ID aktivitas. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Mendapatkan awalan yang digunakan dalam penomoran ulang ID aktivitas. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Mendapatkan akhiran yang digunakan dalam penomoran ulang ID aktivitas. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Mendapatkan nilai yang menunjukkan apakah perlu menomori ulang ID aktivitas. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Mengatur kenaikan yang digunakan dalam penomoran ulang ID aktivitas. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Mengatur awalan yang digunakan dalam penomoran ulang ID aktivitas. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Mengatur akhiran yang digunakan dalam penomoran ulang ID aktivitas. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Mengatur nilai yang menunjukkan apakah perlu melakukan penomoran ulang ID aktivitas. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Menginisialisasi instance baru dari kelas [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Mendapatkan kenaikan yang digunakan dalam penomoran ulang ID aktivitas.

**Returns:**
int - kenaikan yang digunakan dalam penomoran ulang ID aktivitas.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Mendapatkan awalan yang digunakan dalam penomoran ulang ID aktivitas.

**Returns:**
java.lang.String - awalan yang digunakan dalam penomoran ulang ID aktivitas.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Mendapatkan akhiran yang digunakan dalam penomoran ulang ID aktivitas.

**Returns:**
int - akhiran yang digunakan dalam penomoran ulang ID aktivitas.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Mendapatkan nilai yang menunjukkan apakah perlu menomori ulang ID aktivitas.

**Returns:**
boolean - nilai yang menunjukkan apakah perlu melakukan penomoran ulang ID aktivitas.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor.

Perangkat lunak Primavera tidak mendukung penugasan sumber daya ke tugas ringkasan (WBS). Oleh karena itu, ekspor penugasan tersebut dapat menghasilkan file yang tidak valid menurut model Primavera. Jika true, penugasan ke tugas ringkasan akan dilewati selama ekspor. Jika false (nilai default), sebuah pengecualian akan dilemparkan jika penugasan ke tugas ringkasan ditemukan selama ekspor.

**Returns:**
boolean - nilai yang menunjukkan apakah penugasan sumber daya ke tugas ringkasan harus dilewati selama ekspor.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Mengatur kenaikan yang digunakan dalam penomoran ulang ID aktivitas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | kenaikan yang digunakan dalam penomoran ulang ID aktivitas. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Mengatur awalan yang digunakan dalam penomoran ulang ID aktivitas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | awalan yang digunakan dalam penomoran ulang ID aktivitas. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Mengatur akhiran yang digunakan dalam penomoran ulang ID aktivitas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | akhiran yang digunakan dalam penomoran ulang ID aktivitas. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Mengatur nilai yang menunjukkan apakah perlu melakukan penomoran ulang ID aktivitas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah perlu melakukan penomoran ulang ID aktivitas. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor.

Perangkat lunak Primavera tidak mendukung penugasan sumber daya ke tugas ringkasan (WBS). Oleh karena itu, ekspor penugasan tersebut dapat menghasilkan file yang tidak valid menurut model Primavera. Jika true, penugasan ke tugas ringkasan akan dilewati selama ekspor. Jika false (nilai default), sebuah pengecualian akan dilemparkan jika penugasan ke tugas ringkasan ditemukan selama ekspor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah penugasan sumber daya ke tugas ringkasan harus dilewati selama ekspor. |

