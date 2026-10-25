---
title: "SvgOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan menentukan opsi tambahan saat merender halaman proyek ke SVG."
type: docs
weight: 283
url: /id/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Memungkinkan menentukan opsi tambahan saat merender halaman proyek ke SVG.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Menginisialisasi instance baru dari kelas [SvgOptions](../../com.aspose.tasks/svgoptions) yang dapat digunakan untuk menyimpan proyek dalam format SVG. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Mendapatkan callback implementasi yang ditentukan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Mengatur callback implementasi yang ditentukan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Menginisialisasi instance baru dari kelas [SvgOptions](../../com.aspose.tasks/svgoptions) yang dapat digunakan untuk menyimpan proyek dalam format SVG.

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
public final SaveOptions deepClone()
```


Dicadangkan untuk penggunaan internal.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Mendapatkan callback implementasi yang ditentukan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek.

--------------------

Saat ini penggunaan kuas gradien tidak didukung untuk rendering ke SVG.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Mengatur callback implementasi yang ditentukan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | callback implementasi yang ditentukan pengguna yang digunakan untuk mendapatkan aliran output untuk setiap halaman yang dirender. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Menentukan apakah akan menggunakan kuas gradien saat merender tata letak proyek.

--------------------

Saat ini penggunaan kuas gradien tidak didukung untuk rendering ke SVG.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menggunakan kuas gradien saat merender tata letak proyek. |

