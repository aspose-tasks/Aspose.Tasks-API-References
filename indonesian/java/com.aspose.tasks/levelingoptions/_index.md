---
title: "LevelingOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan parameter penyeimbangan sumber daya."
type: docs
weight: 142
url: /id/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Memungkinkan untuk menentukan parameter penyeimbangan sumber daya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Menginisialisasi instance baru dari kelas [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Mendapatkan token yang dapat digunakan untuk membatalkan operasi leveling proyek. |
| [getFinishDate()](#getFinishDate--) | Mendapatkan tanggal akhir periode leveling. |
| [getLevelingOrder()](#getLevelingOrder--) | Mendapatkan urutan di mana algoritma leveling menunda tugas yang memiliki alokasi berlebih. |
| [getMessageHandler()](#getMessageHandler--) | Mendapatkan callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama leveling sumber daya. |
| [getMessageLevel()](#getMessageLevel--) | Mendapatkan tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama leveling sumber daya. |
| [getResources()](#getResources--) | Mendapatkan daftar sumber daya yang akan diseimbangkan. |
| [getStartDate()](#getStartDate--) | Mendapatkan tanggal mulai periode penyeimbangan. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Mengatur token yang dapat digunakan untuk membatalkan operasi penyeimbangan proyek. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Mengatur tanggal akhir periode penyeimbangan. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | Urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Mengatur callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Mengatur tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama penyeimbangan sumber daya. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Mengatur daftar sumber daya yang akan diseimbangkan. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Mengatur tanggal mulai periode penyeimbangan. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Menginisialisasi instance baru dari kelas [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Mendapatkan token yang dapat digunakan untuk membatalkan operasi leveling proyek.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Mendapatkan tanggal akhir periode penyeimbangan. Nilai default adalah tanggal selesai proyek.

**Returns:**
java.util.Date - tanggal akhir periode penyeimbangan.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Mendapatkan urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih. Setelah menentukan tugas yang menyebabkan alokasi berlebih dan tugas mana yang dapat ditunda, urutan yang ditentukan digunakan untuk menentukan tugas mana yang harus ditunda pertama.

**Returns:**
int - urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Mendapatkan callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama leveling sumber daya.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Mendapatkan tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama leveling sumber daya.

**Returns:**
int - tingkat pesan log yang dikeluarkan oleh Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Mendapatkan daftar sumber daya yang akan diseimbangkan. Jika null diatur, semua sumber daya proyek akan diseimbangkan.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - daftar sumber daya yang akan diseimbangkan.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Mendapatkan tanggal mulai periode penyeimbangan. Nilai default adalah tanggal mulai proyek.

**Returns:**
java.util.Date - tanggal mulai periode penyeimbangan.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Mengatur token yang dapat digunakan untuk membatalkan operasi penyeimbangan proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | token yang dapat digunakan untuk membatalkan operasi penyeimbangan proyek. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Mengatur tanggal akhir periode penyeimbangan. Nilai default adalah tanggal selesai proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal akhir periode penyeimbangan. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


Urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih. Setelah menentukan tugas yang menyebabkan alokasi berlebih dan tugas mana yang dapat ditunda, urutan yang ditentukan digunakan untuk menentukan tugas mana yang harus ditunda pertama.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | urutan di mana algoritma penyeimbangan menunda tugas yang memiliki alokasi berlebih. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Mengatur callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose.Tasks selama penyeimbangan sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | callback penangan pesan yang dapat digunakan untuk menyaring pesan log yang dihasilkan oleh Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Mengatur tingkat pesan log yang dikeluarkan oleh Aspose.Tasks selama penyeimbangan sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tingkat pesan log yang dikeluarkan oleh Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Mengatur daftar sumber daya yang akan disejajarkan. Jika null diatur, semua sumber daya proyek akan disejajarkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.List&lt;com.aspose.tasks.Resource&gt; | daftar sumber daya yang akan disejajarkan. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Mengatur tanggal mulai periode penyelarasan. Nilai default adalah tanggal mulai proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal mulai periode penyelarasan. |

