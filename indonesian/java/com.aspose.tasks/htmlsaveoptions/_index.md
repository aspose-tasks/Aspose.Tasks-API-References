---
title: "HtmlSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke HTML."
type: docs
weight: 132
url: /id/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat merender halaman proyek ke HTML.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Menginisialisasi sebuah instance baru dari kelas [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Mendapatkan awalan gaya CSS. |
| [getExportCss()](#getExportCss--) | Mendapatkan cara CSS diekspor. |
| [getExportFonts()](#getExportFonts--) | Mendapatkan cara font diekspor. |
| [getExportImages()](#getExportImages--) | Mendapatkan cara gambar diekspor. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Mendapatkan jenis font face. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan font. |
| [getFontSettings()](#getFontSettings--) | Menentukan pengaturan font yang digunakan saat merender tampilan proyek. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan font. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Mendapatkan nilai yang menunjukkan apakah menyertakan nama proyek di header halaman HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Mendapatkan nilai yang menunjukkan apakah menyertakan nama proyek di judul HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Mendapatkan callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [getPages()](#getPages--) | Mendapatkan daftar nomor halaman yang akan disimpan saat merender tata letak proyek. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Mendapatkan nilai yang menunjukkan apakah menggunakan kuas gradien saat merender tata letak proyek. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Mengatur awalan gaya CSS. |
| [setExportCss(int value)](#setExportCss-int-) | Mengatur cara CSS diekspor. |
| [setExportFonts(int value)](#setExportFonts-int-) | Mengatur cara font diekspor. |
| [setExportImages(int value)](#setExportImages-int-) | Mengatur cara gambar diekspor. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Mengatur tipe font face. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan font. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan font. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan nama proyek dalam header halaman HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan nama proyek dalam judul HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Mengatur callback yang didefinisikan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Mengatur daftar nomor halaman yang akan disimpan saat merender tata letak proyek. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Menginisialisasi sebuah instance baru dari kelas [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Mendapatkan awalan gaya CSS.

**Returns:**
java.lang.String - awalan gaya CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Mendapatkan cara CSS diekspor.

**Returns:**
int - cara CSS diekspor.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Mendapatkan cara font diekspor.

**Returns:**
int - cara font diekspor.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Mendapatkan cara gambar diekspor.

**Returns:**
int - cara gambar diekspor.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Mendapatkan jenis font face.

Nilai: Tipe font face.

**Returns:**
int - tipe font face.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan font.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Menentukan pengaturan font yang digunakan saat merender tampilan proyek.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Mendapatkan callback yang dipanggil untuk membuat sumber daya menyimpan font.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan nama proyek di header halaman HTML.

**Returns:**
boolean - nilai yang menunjukkan apakah menyertakan nama proyek dalam header halaman HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan nama proyek di judul HTML.

**Returns:**
boolean - nilai yang menunjukkan apakah menyertakan nama proyek dalam judul HTML.
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


Mendapatkan daftar nomor halaman yang akan disimpan saat merender tata letak proyek.

--------------------

Semua halaman proyek akan disimpan jika daftar ini kosong.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - daftar nomor halaman yang akan disimpan saat merender tata letak proyek.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Mendapatkan nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Returns:**
boolean - nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Mendapatkan nilai yang menunjukkan apakah menggunakan kuas gradien saat merender tata letak proyek.

--------------------

Penggunaan kuas gradien saat ini tidak didukung saat merender ke HTML.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan CSS.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | callback yang dipanggil untuk membuat sumber daya menyimpan CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Mengatur awalan gaya CSS.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Awalan gaya CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Mengatur cara CSS diekspor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | cara CSS diekspor. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Mengatur cara font diekspor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | cara font diekspor. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Mengatur cara gambar diekspor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | cara gambar diekspor. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Mengatur tipe font face.

Nilai: Tipe font face.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jenis font face. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | callback yang dipanggil untuk membuat sumber daya menyimpan font. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Mengatur callback yang dipanggil untuk membuat sumber daya menyimpan font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | callback yang dipanggil untuk membuat sumber daya menyimpan font. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan nama proyek dalam header halaman HTML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menyertakan nama proyek di header halaman HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan nama proyek dalam judul HTML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menyertakan nama proyek di judul HTML. |

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


Mengatur daftar nomor halaman yang akan disimpan saat merender tata letak proyek.

--------------------

Semua halaman proyek akan disimpan jika daftar ini kosong.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.List&lt;java.lang.Integer&gt; | daftar nomor halaman yang akan disimpan saat merender tata letak proyek. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Mengatur nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah celah antara tugas terakhir dan footer harus dikurangi. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek.

--------------------

Penggunaan kuas gradien saat ini tidak didukung saat merender ke HTML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menggunakan kuas gradien saat merender tata letak proyek. |

