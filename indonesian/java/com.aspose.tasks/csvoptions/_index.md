---
title: "CsvOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke CSV."
type: docs
weight: 56
url: /id/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke CSV.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Menginisialisasi instance baru dari kelas [CsvOptions](../../com.aspose/tasks/csvoptions) yang dapat digunakan untuk menyimpan proyek dalam format CSV. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Mendapatkan kategori data yang akan disimpan. |
| [getEncoding()](#getEncoding--) | Mendapatkan encoding untuk menyimpan CSV dengan. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Mendapatkan nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Mendapatkan pembatas teks. |
| [getView()](#getView--) | Mendapatkan daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | Mengatur kategori data yang akan disimpan. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur encoding untuk menyimpan CSV dengan. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Mengatur pembatas teks. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Mengatur daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Menginisialisasi instance baru dari kelas [CsvOptions](../../com.aspose/tasks/csvoptions) yang dapat digunakan untuk menyimpan proyek dalam format CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Mendapatkan kategori data yang akan disimpan.

**Returns:**
int - kategori data yang akan disimpan.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan encoding untuk menyimpan CSV dengan.

**Returns:**
java.nio.charset.Charset - encoding untuk menyimpan CSV dengan.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE).

**Returns:**
boolean - nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Mendapatkan pembatas teks.

**Returns:**
int - pembatas teks.
### getView() {#getView--}
```
public final ProjectView getView()
```


Mendapatkan daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. Jika tidak diatur maka kolom default akan disimpan.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Mengatur kategori data yang akan disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | kategori data yang akan disimpan. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Mengatur encoding untuk menyimpan CSV dengan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | encoding untuk menyimpan CSV dengan. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Mengatur pembatas teks.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pembatas teks. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Mengatur daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. Jika tidak diatur maka kolom default akan disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | daftar kolom tampilan ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) untuk disimpan ke format XLSX. |

