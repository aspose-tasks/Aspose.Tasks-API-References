---
title: "ResourceSavingArgs"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas ini mewakili sekumpulan data yang terkait dengan penyimpanan file sumber eksternal yang terjadi selama konversi ke format HTML."
type: docs
weight: 254
url: /id/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Kelas ini mewakili sekumpulan data yang terkait dengan penyimpanan file sumber daya eksternal yang terjadi selama konversi ke format HTML.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Tutup aliran jika KeepStreamOpen bernilai false, jika tidak, bersihkan aliran tersebut. |
| [getFileName()](#getFileName--) | Mendapatkan nama file yang diharapkan yang berasal dari konverter ke kode metode khusus. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Mendapatkan nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai. |
| [getStream()](#getStream--) | Mendapatkan konten biner dari file yang disimpan. |
| [getUri()](#getUri--) | Mendapatkan URI sumber daya. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Mengatur nama file yang diharapkan yang berasal dari konverter ke kode metode khusus. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Mengatur nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Mengatur konten biner dari file yang disimpan. |
| [setUri(String value)](#setUri-java.lang.String-) | Mengatur URI sumber daya. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Tutup aliran jika KeepStreamOpen bernilai false, jika tidak, bersihkan aliran tersebut.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Mendapatkan nama file yang diharapkan yang berasal dari konverter ke kode metode khusus. Dapat digunakan dalam kode khusus untuk memutuskan bagaimana memproses atau dimana menyimpan file tersebut.

**Returns:**
java.lang.String - nama file yang diharapkan yang berasal dari konverter ke kode metode khusus.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Mendapatkan nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai.

**Returns:**
boolean - nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Mendapatkan konten biner dari file yang disimpan.

**Returns:**
java.io.OutputStream - konten biner dari file yang disimpan.
### getUri() {#getUri--}
```
public final String getUri()
```


Mendapatkan URI sumber daya.

**Returns:**
java.lang.String - URI sumber daya.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Mengatur nama file yang diharapkan yang berasal dari konverter ke kode metode khusus. Dapat digunakan dalam kode khusus untuk memutuskan bagaimana memproses atau dimana menyimpan file tersebut.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama file yang diharapkan yang berasal dari konverter ke kode metode khusus. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Mengatur nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah aliran akan tetap terbuka setelah penyimpanan sumber selesai. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Mengatur konten biner dari file yang disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.io.OutputStream | konten biner dari file yang disimpan. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Mengatur URI sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | URI sumber daya. |

