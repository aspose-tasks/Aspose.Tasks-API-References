---
title: "LoadOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan parameter pemuatan tambahan saat memuat proyek dari berkas atau aliran."
type: docs
weight: 148
url: /id/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Memungkinkan untuk menentukan parameter pemuatan tambahan saat memuat proyek dari berkas atau aliran.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Menginisialisasi sebuah instance baru dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Mendapatkan token yang dapat digunakan untuk membatalkan operasi pemuatan proyek. |
| [getEncoding()](#getEncoding--) | Mendapatkan enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | Mendapatkan metode callback untuk menangani kesalahan parsing xml. |
| [getPassword()](#getPassword--) | Mendapatkan kata sandi perlindungan. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Mendapatkan instance tertentu dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Mengatur token yang dapat digunakan untuk membatalkan operasi pemuatan proyek. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Mengatur metode callback untuk menangani kesalahan parsing xml. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Mengatur kata sandi perlindungan. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Mengatur instance tertentu dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Menginisialisasi sebuah instance baru dari kelas [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Mendapatkan token yang dapat digunakan untuk membatalkan operasi pemuatan proyek.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. Enkoding default adalah UTF8.

**Returns:**
java.nio.charset.Charset - enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Mendapatkan metode callback untuk menangani kesalahan parsing xml.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Mendapatkan kata sandi perlindungan.

**Returns:**
java.lang.String - sebuah kata sandi perlindungan.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Mendapatkan instance tertentu dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Mengatur token yang dapat digunakan untuk membatalkan operasi pemuatan proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | token yang dapat digunakan untuk membatalkan operasi pemuatan proyek. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Mengatur enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. Enkoding default adalah UTF8.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | enkoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Mengatur metode callback untuk menangani kesalahan parsing xml.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | metode callback untuk menangani kesalahan parsing xml. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Mengatur kata sandi perlindungan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi perlindungan. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Mengatur instance tertentu dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | instance tertentu dari kelas [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) yang dapat digunakan untuk menyesuaikan perilaku pemuatan format Primavera (Primavera P6 XER atau Primavera P6 Xml). |

