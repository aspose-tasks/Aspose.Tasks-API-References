---
title: "PageSettings"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pengaturan pencetakan untuk halaman tampilan proyek."
type: docs
weight: 181
url: /id/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Mewakili pengaturan pencetakan untuk halaman tampilan proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PageSettings()](#PageSettings--) | Menginisialisasi instance baru dari kelas [PageSettings](../../com.aspose.tasks/pagesettings). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Mendapatkan nilai yang menunjukkan apakah harus menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Mendapatkan nomor halaman pertama untuk pencetakan. |
| [getPagesInHeight()](#getPagesInHeight--) | Mendapatkan jumlah halaman dalam tinggi yang akan dicetak. |
| [getPagesInWidth()](#getPagesInWidth--) | Mendapatkan jumlah halaman dalam lebar yang akan dicetak. |
| [getPaperSize()](#getPaperSize--) | Mendapatkan ukuran kertas. |
| [getPaperSizeId()](#getPaperSizeId--) | Mendapatkan integer yang mewakili salah satu nilai PrinterPaperSize atau ID ukuran halaman khusus. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Mendapatkan persentase dari ukuran normal untuk menyesuaikan pencetakan. |
| [isPortrait()](#isPortrait--) | Mendapatkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Mengatur nilai yang menunjukkan apakah harus menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Mengatur nomor halaman pertama untuk pencetakan. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Mengatur jumlah halaman dalam tinggi yang akan dicetak. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Mengatur jumlah halaman dalam lebar yang akan dicetak. |
| [setPaperSize(int value)](#setPaperSize-int-) | Mengatur ukuran kertas. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Mengatur integer yang mewakili salah satu nilai PrinterPaperSize atau ID ukuran halaman khusus. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Mengatur persentase dari ukuran normal untuk menyesuaikan pencetakan. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Menginisialisasi instance baru dari kelas [PageSettings](../../com.aspose/tasks/pagesettings). Mewakili pengaturan pencetakan untuk sebuah halaman tampilan proyek.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Mendapatkan nilai yang menunjukkan apakah harus menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal.

--------------------

Tidak efektif ketika proyek dirender dalam format HTML.

**Returns:**
boolean - nilai yang menunjukkan apakah harus menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Mendapatkan nomor halaman pertama untuk pencetakan.

**Returns:**
short - nomor halaman pertama untuk pencetakan.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Mendapatkan jumlah halaman dalam tinggi yang akan dicetak.

**Returns:**
int - jumlah halaman dalam tinggi yang akan dicetak.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Mendapatkan jumlah halaman dalam lebar yang akan dicetak.

**Returns:**
int - jumlah halaman dalam lebar yang akan dicetak.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Mendapatkan ukuran kertas. Bisa menjadi salah satu nilai dari enumerasi [PrinterPaperSize](../../com.aspose/tasks/printerpapersize).

**Returns:**
int - ukuran kertas.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Mendapatkan integer yang mewakili salah satu nilai PrinterPaperSize atau ID ukuran halaman khusus. Nilai ini dapat digunakan untuk mendapatkan PaperSize dari pengaturan OS ().

**Returns:**
int - sebuah integer yang mewakili salah satu nilai PrinterPaperSize atau id ukuran halaman khusus.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Mendapatkan persentase dari ukuran normal untuk menyesuaikan pencetakan.

**Returns:**
int - persentase ukuran normal untuk menyesuaikan pencetakan.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Mendapatkan nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.

--------------------

Berlaku selama rendering ketika SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Mengatur nilai yang menunjukkan apakah harus menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal.

--------------------

Tidak efektif ketika proyek dirender dalam format HTML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | boolean | nilai yang menunjukkan apakah akan menyesuaikan pencetakan ke persentase yang ditentukan (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) dari ukuran normal. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Mengatur nomor halaman pertama untuk pencetakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | short | nomor halaman pertama untuk pencetakan. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Mengatur jumlah halaman dalam tinggi yang akan dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah halaman dalam tinggi yang akan dicetak. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Mengatur jumlah halaman dalam lebar yang akan dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah halaman dalam lebar yang akan dicetak. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Mengatur ukuran kertas. Bisa menjadi salah satu nilai dari enumerasi [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | ukuran kertas. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Mengatur sebuah integer yang mewakili salah satu nilai PrinterPaperSize atau id ukuran halaman khusus. Nilai ini dapat digunakan untuk mendapatkan PaperSize dari pengaturan OS ().

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sebuah integer yang mewakili salah satu nilai PrinterPaperSize atau id ukuran halaman khusus. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Mengatur persentase dari ukuran normal untuk menyesuaikan pencetakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | persentase ukuran normal untuk menyesuaikan pencetakan. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Mengatur nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape.

--------------------

Berlaku selama rendering ketika SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah orientasi halaman portrait; mengembalikan false jika orientasi halaman landscape. |

