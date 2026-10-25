---
title: "ProjectServerCredentials"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kredensial yang digunakan untuk terhubung ke Project Online atau instance on-premise Project Server."
type: docs
weight: 225
url: /id/java/com.aspose.tasks/projectservercredentials/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerCredentials
```

Kredensial yang digunakan untuk terhubung ke Project Online atau instance on-premise Project Server.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProjectServerCredentials(String siteUrl, String authToken)](#ProjectServerCredentials-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk situs PWA (Project Web Access) SharePoint. |
| [ProjectServerCredentials(String siteUrl, String userName, String password)](#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-) | Menginisialisasi instance baru dari kelas [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) menggunakan URL situs SharePoint, nama pengguna, dan kata sandi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAuthToken()](#getAuthToken--) | Mendapatkan token otorisasi untuk instance SharePoint. |
| [getSiteUrl()](#getSiteUrl--) | Mendapatkan URL PWA di situs SharePoint atau URL Project Server lokal. |
| [getUserName()](#getUserName--) | Mendapatkan nama pengguna untuk situs SharePoint. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance ini. |
### ProjectServerCredentials(String siteUrl, String authToken) {#ProjectServerCredentials-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String authToken)
```


Menginisialisasi instance baru dari kelas [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk situs PWA (Project Web Access) SharePoint.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| siteUrl | java.lang.String | URL API PWA (Project Web Access) dari Project Online. |
|  | authToken | java.lang.String | Token otorisasi (SPOIDCRL) untuk situs PWA (Project Web Access) SharePoint. |

--------------------

Gunakan konstruktor ini untuk terhubung ke ProjectOnline ketika Anda sudah memiliki AuthToken untuk situs SharePoint Online Anda. |

### ProjectServerCredentials(String siteUrl, String userName, String password) {#ProjectServerCredentials-java.lang.String-java.lang.String-java.lang.String-}
```
public ProjectServerCredentials(String siteUrl, String userName, String password)
```


Menginisialisasi instance baru dari kelas [ProjectServerCredentials](../../com.aspose/tasks/projectservercredentials) menggunakan URL situs SharePoint, nama pengguna, dan kata sandi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| siteUrl | java.lang.String | URL API PWA (Project Web Access) dari Project Online. |
| userName | java.lang.String | Nama pengguna untuk situs SharePoint. |
|  | password | java.lang.String | Kata sandi untuk situs SharePoint. |

--------------------

Gunakan konstruktor ini untuk terhubung ke ProjectOnline. Harap perhatikan bahwa autentikasi warisan harus diaktifkan di portal Azure Anda dan pusat admin Office 365. |

### getAuthToken() {#getAuthToken--}
```
public final String getAuthToken()
```


Mendapatkan token otorisasi untuk instance SharePoint.

**Returns:**
java.lang.String - token otorisasi untuk instance SharePoint.
### getSiteUrl() {#getSiteUrl--}
```
public final String getSiteUrl()
```


Mendapatkan URL PWA di situs SharePoint atau URL Project Server lokal. Misalnya, https://your\\_company\\_name.sharepoint.com/sites/pwa\";

**Returns:**
java.lang.String - URL PWA di situs SharePoint atau URL Project Server lokal.
### getUserName() {#getUserName--}
```
public final String getUserName()
```


Mendapatkan nama pengguna untuk situs SharePoint.

**Returns:**
java.lang.String - nama pengguna untuk situs SharePoint.
### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari instance ini.

**Returns:**
java.lang.String - representasi string dari instansi ini.
