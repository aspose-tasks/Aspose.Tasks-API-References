---
title: "Aspose::Tasks::ProjectServerCredentials::ProjectServerCredentials konstruktor"
linktitle: "ProjectServerCredentials"
articleTitle: "ProjectServerCredentials"
second_title: "Aspose.Tasks untuk C++"
description: "Menginisialisasi sebuah instance baru dari kelas ProjectServerCredentials menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk PWA ( Project Web Access) SharePoint"
type: docs
weight: 10
url: /id/cpp/aspose.tasks/projectservercredentials/projectservercredentials/
---

## ProjectServerCredentials (1 of 3) {#projectservercredentials_1}

Menginisialisasi instance baru dari kelas ProjectServerCredentials menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk situs PWA (Project Web Access) SharePoint.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & authToken)
```

| Parameter | Deskripsi |
| --- | --- |
| siteUrl | URL PWA ( Project Web Access) API dari Project Online. |
| authToken | Token otorisasi (SPOIDCRL) untuk PWA ( Project Web Access) situs SharePoint. |

---

## ProjectServerCredentials (2 of 3) {#projectservercredentials_2}

Menginisialisasi sebuah instance baru dari kelas ProjectServerCredentials menggunakan URL situs SharePoint, nama pengguna, dan kata sandi.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::String & userName, const System::String & password)
```

| Parameter | Deskripsi |
| --- | --- |
| siteUrl | URL PWA ( Project Web Access) API dari Project Online. |
| userName | Nama pengguna untuk situs SharePoint. |
| password | Kata sandi untuk situs SharePoint. |

---

## ProjectServerCredentials (3 of 3) {#projectservercredentials_3}

Menginisialisasi sebuah instance baru dari kelas ProjectServerCredentials menggunakan URL endpoint Project Web Access dan kredensial jaringan.

**Returns:** Aspose::Tasks::

```cpp
ProjectServerCredentials(const System::String & siteUrl, const System::SharedPtr< System::Net::NetworkCredential > & credentials)
```

| Parameter | Deskripsi |
| --- | --- |
| siteUrl | URL endpoint project web access. |
| kredensial | Kredensial yang digunakan untuk masuk ke endpoint Project Web Access. |

