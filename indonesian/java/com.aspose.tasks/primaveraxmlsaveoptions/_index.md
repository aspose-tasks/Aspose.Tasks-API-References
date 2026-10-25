---
title: "PrimaveraXmlSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera xml."
type: docs
weight: 212
url: /id/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke format Primavera xml.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Menginisialisasi instance baru dari kelas [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Mendapatkan nilai yang menunjukkan apakah akan menyimpan tugas akar atau tidak. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Mengatur nilai yang menunjukkan apakah akan menyimpan tugas akar atau tidak. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Mengatur nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Menginisialisasi instance baru dari kelas [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Mendapatkan nilai yang menunjukkan apakah akan menyimpan tugas akar atau tidak.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menyimpan tugas root atau tidak.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Mendapatkan nilai yang menunjukkan apakah penugasan sumber daya ke tugas rangkuman harus dilewati selama ekspor.

Perangkat lunak Primavera tidak mendukung penugasan sumber daya ke tugas ringkasan (WBS). Oleh karena itu, ekspor penugasan tersebut dapat menghasilkan file yang tidak valid menurut model Primavera. Jika true, penugasan ke tugas ringkasan akan dilewati selama ekspor. Jika false (nilai default), sebuah pengecualian akan dilemparkan jika penugasan ke tugas ringkasan ditemukan selama ekspor.

**Returns:**
boolean - nilai yang menunjukkan apakah penugasan sumber daya ke tugas ringkasan harus dilewati selama ekspor.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menyimpan tugas akar atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menyimpan tugas root atau tidak. |

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

