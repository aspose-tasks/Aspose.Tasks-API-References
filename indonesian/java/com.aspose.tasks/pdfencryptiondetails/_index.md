---
title: "PdfEncryptionDetails"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Berisi detail untuk enkripsi PDF."
type: docs
weight: 189
url: /id/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Berisi detail untuk enkripsi PDF.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Menginisialisasi sebuah instance baru dari kelas [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Mendapatkan mode enkripsi. |
| [getOwnerPassword()](#getOwnerPassword--) | Mendapatkan kata sandi Owner. |
| [getPermissions()](#getPermissions--) | Mendapatkan izin. |
| [getUserPassword()](#getUserPassword--) | Mendapatkan kata sandi User. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Mengatur mode enkripsi. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Mengatur kata sandi Owner. |
| [setPermissions(int value)](#setPermissions-int-) | Mengatur izin. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Mengatur kata sandi User. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Menginisialisasi sebuah instance baru dari kelas [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| userPassword | java.lang.String | Kata sandi user yang memungkinkan membuka dokumen yang dilindungi. |
| ownerPassword | java.lang.String | Kata sandi owner yang memungkinkan membuka dokumen yang dilindungi. |
| encryptionAlgorithm | int | Instansi [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) yang menunjukkan algoritma enkripsi. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Mendapatkan mode enkripsi.

**Returns:**
int - mode enkripsi.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Mendapatkan kata sandi Owner.

--------------------

Membuka dokumen dengan kata sandi owner yang benar (dengan asumsi tidak sama dengan kata sandi user) memungkinkan akses penuh (owner) ke dokumen. Akses tak terbatas ini mencakup kemampuan untuk mengubah kata sandi dokumen\\u2019s dan izin akses.

**Returns:**
java.lang.String - kata sandi Owner.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Mendapatkan izin.

**Returns:**
int - izin.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Mendapatkan kata sandi User.

--------------------

Membuka dokumen dengan kata sandi user yang benar (atau membuka dokumen yang tidak memiliki kata sandi user) memungkinkan operasi tambahan dilakukan sesuai dengan izin akses user yang ditentukan dalam kamus enkripsi dokumen\\u2019s.

**Returns:**
java.lang.String - kata sandi Pengguna.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Mengatur mode enkripsi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | mode enkripsi. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Mengatur kata sandi Owner.

--------------------

Membuka dokumen dengan kata sandi owner yang benar (dengan asumsi tidak sama dengan kata sandi user) memungkinkan akses penuh (owner) ke dokumen. Akses tak terbatas ini mencakup kemampuan untuk mengubah kata sandi dokumen\\u2019s dan izin akses.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi Pemilik. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Mengatur izin.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | izin. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Mengatur kata sandi User.

--------------------

Membuka dokumen dengan kata sandi user yang benar (atau membuka dokumen yang tidak memiliki kata sandi user) memungkinkan operasi tambahan dilakukan sesuai dengan izin akses user yang ditentukan dalam kamus enkripsi dokumen\\u2019s.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi Pengguna. |

