---
title: "ImageSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke gambar."
type: docs
weight: 134
url: /id/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke gambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Menginisialisasi instance baru dari kelas [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) yang dapat digunakan untuk menyimpan gambar yang dirender dalam format TIFF, PNG, BMP, atau JPEG. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Menentukan pengaturan font yang digunakan saat merender tampilan proyek. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Mendapatkan resolusi horizontal dalam dpi. |
| [getJpegQuality()](#getJpegQuality--) | Mendapatkan kualitas JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Mendapatkan callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [getPages()](#getPages--) | Mendapatkan daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. |
| [getPixelFormat()](#getPixelFormat--) | Mendapatkan format data warna untuk setiap piksel dalam gambar. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [getTiffCompression()](#getTiffCompression--) | Mendapatkan jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | Mendapatkan resolusi vertikal dalam dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Mengatur resolusi horizontal dalam dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Mengatur kualitas JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Mengatur daftar nomor halaman yang akan disimpan saat menyimpan tata letak proyek ke file terpisah. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Mengatur format data warna untuk setiap piksel dalam gambar. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Mengatur jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Mengatur resolusi vertikal dalam dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Menginisialisasi instance baru dari kelas [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) yang dapat digunakan untuk menyimpan gambar yang dirender dalam format TIFF, PNG, BMP, atau JPEG.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| saveFormat | int | Bisa berupa TIFF, PNG, BMP, atau JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Menentukan pengaturan font yang digunakan saat merender tampilan proyek.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Mendapatkan resolusi horizontal dalam dpi.

**Returns:**
float - resolusi horizontal dalam dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Mendapatkan kualitas JPEG. Rentang nilai yang diizinkan adalah 0..100.

**Returns:**
int - kualitas JPEG.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Mendapatkan callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender.

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
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Mendapatkan format data warna untuk setiap piksel dalam gambar.

**Returns:**
int - format data warna untuk setiap piksel dalam gambar.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Returns:**
boolean - nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Mendapatkan jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF.

--------------------

Berpengaruh hanya saat menyimpan ke TIFF. Nilai default adalah `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Mendapatkan resolusi vertikal dalam dpi.

**Returns:**
float - resolusi vertikal dalam dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Mengatur resolusi horizontal dalam dpi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | resolusi horizontal dalam dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Mengatur kualitas JPEG. Rentang nilai yang diizinkan adalah 0..100.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | kualitas JPEG. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender.

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

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Mengatur format data warna untuk setiap piksel dalam gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | format data warna untuk setiap piksel dalam gambar. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Mengatur jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF.

--------------------

Berpengaruh hanya saat menyimpan ke TIFF. Nilai default adalah `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jenis kompresi yang diterapkan saat menyimpan gambar yang dihasilkan ke format TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Mengatur resolusi vertikal dalam dpi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | resolusi vertikal dalam dpi. |

