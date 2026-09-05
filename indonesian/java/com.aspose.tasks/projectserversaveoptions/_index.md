---
title: "ProjectServerSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan opsi tambahan ketika proyek disimpan ke Project Server atau Project Online."
type: docs
weight: 227
url: /id/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Memungkinkan untuk menentukan opsi tambahan ketika proyek disimpan ke Project Server atau Project Online.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Menginisialisasi instance baru dari kelas [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Mendapatkan interval antara permintaan status pekerjaan antrian. |
| [getProjectGuid()](#getProjectGuid--) | Mendapatkan pengidentifikasi unik dari sebuah proyek. |
| [getProjectName()](#getProjectName--) | Mendapatkan nama proyek yang ditampilkan dalam daftar proyek Project Server \\ Project Online. |
| [getTimeout()](#getTimeout--) | Mendapatkan batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrian Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Mengatur interval antara permintaan status pekerjaan antrian. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Mengatur pengidentifikasi unik dari sebuah proyek. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Mengatur nama proyek yang ditampilkan dalam daftar proyek Project Server \\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | Mengatur batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrian Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Menginisialisasi instance baru dari kelas [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Mendapatkan interval antara permintaan status pekerjaan antrian. Nilai default adalah 2 detik.

**Returns:**
double - interval antara permintaan status pekerjaan antrian.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Mendapatkan pengidentifikasi unik dari sebuah proyek. Harus unik dalam instance Project Server \\ Project Online.

**Returns:**
java.util.UUID - pengidentifikasi unik dari sebuah proyek.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Mendapatkan nama proyek yang ditampilkan dalam daftar proyek Project Server \\ Project Online. Harus unik dalam instance Project Server \\ Project Online. Jika nilai dihilangkan, nilai properti Prj.Name akan digunakan sebagai gantinya.

**Returns:**
java.lang.String - nama proyek yang ditampilkan dalam daftar proyek Project Server \\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Mendapatkan batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrian Project Server. Nilai default untuk properti ini adalah 1 menit.

--------------------

Waktu pemrosesan mungkin lebih lama untuk proyek besar atau bila instance Project Server terlalu sibuk menanggapi permintaan lain.

**Returns:**
double - batas waktu yang digunakan saat menunggu pemrosesan permintaan simpan proyek oleh layanan pemrosesan antrean Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Mengatur interval antara permintaan status pekerjaan antrean. Nilai default adalah 2 detik.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | interval antara permintaan status pekerjaan antrean. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Mengatur pengidentifikasi unik sebuah proyek. Harus unik dalam instance Project Server \ Project Online.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.UUID | pengidentifikasi unik sebuah proyek. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Mengatur nama proyek yang ditampilkan dalam daftar proyek Project Server \ Project Online. Harus unik dalam instance Project Server \ Project Online. Jika nilai dihilangkan, nilai properti Prj.Name akan digunakan sebagai gantinya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama proyek yang ditampilkan dalam daftar proyek Project Server \ Project Online. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Mengatur batas waktu yang digunakan saat menunggu pemrosesan permintaan simpan proyek oleh layanan pemrosesan antrean Project Server. Nilai default untuk properti ini adalah 1 menit.

--------------------

Waktu pemrosesan mungkin lebih lama untuk proyek besar atau bila instance Project Server terlalu sibuk menanggapi permintaan lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | batas waktu yang digunakan saat menunggu pemrosesan permintaan simpan proyek oleh layanan pemrosesan antrean Project Server. |

