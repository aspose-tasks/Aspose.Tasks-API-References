---
title: "PdfSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF."
type: docs
weight: 191
url: /id/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke PDF.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Menginisialisasi instance baru dari kelas [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) yang dapat digunakan untuk menyimpan dokumen dalam format [SaveFileFormat](../../com.aspose.tasks/savefileformat). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Mendapatkan tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Mendapatkan detail enkripsi. |
| [getFontSettings()](#getFontSettings--) | Menentukan pengaturan font yang digunakan saat merender tampilan proyek. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Mendapatkan callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [getPages()](#getPages--) | Mendapatkan daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Mendapatkan nilai yang menunjukkan apakah halaman proyek akan disimpan ke file terpisah. |
| [getTextCompression()](#getTextCompression--) | Mendapatkan tipe kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. |
| [setCompliance(int value)](#setCompliance-int-) | Mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Mengatur detail enkripsi. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Mengatur nilai yang menunjukkan apakah halaman proyek akan disimpan ke file terpisah. |
| [setTextCompression(int value)](#setTextCompression-int-) | Mengatur tipe kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Menginisialisasi instance baru dari kelas [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) yang dapat digunakan untuk menyimpan dokumen dalam format [SaveFileFormat](../../com.aspose.tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Dicadangkan untuk penggunaan internal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Dicadangkan untuk penggunaan internal.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Mendapatkan tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Default adalah [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\\#Pdf15).

**Returns:**
int - tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Mendapatkan detail enkripsi. Jika tidak diatur, maka tidak akan ada enkripsi yang dilakukan.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Menentukan pengaturan font yang digunakan saat merender tampilan proyek.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Mendapatkan callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. Berlaku ketika opsi `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\\#setSaveToSeparateFiles-boolean-)) digunakan.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Mendapatkan daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah.

--------------------

Semua halaman akan disimpan jika daftar ini kosong.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Returns:**
boolean - nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Mendapatkan nilai yang menunjukkan apakah halaman proyek akan disimpan ke file terpisah.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menyimpan halaman proyek ke file terpisah.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Mendapatkan jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Defaultnya adalah [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Mengatur tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. Defaultnya adalah [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tingkat kepatuhan yang diinginkan untuk dokumen PDF yang dihasilkan. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Mengatur detail enkripsi. Jika tidak diatur, maka tidak akan ada enkripsi yang dilakukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | detail enkripsi. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. Berlaku ketika opsi `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah.

--------------------

Semua halaman akan disimpan jika daftar ini kosong.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.List&lt;java.lang.Integer&gt; | daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Mengatur nilai yang menunjukkan apakah halaman proyek akan disimpan ke file terpisah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menyimpan halaman proyek ke file terpisah. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Mengatur jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. Defaultnya adalah [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jenis kompresi yang akan digunakan untuk semua aliran konten kecuali gambar. |

