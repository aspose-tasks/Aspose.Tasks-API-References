---
title: "Kelas ProjectInfo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectInfo. Informasi singkat tentang proyek yang dipublikasikan tersedia di Project Online."
type: docs
weight: 1470
url: /id/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Info singkat tentang proyek yang dipublikasikan tersedia di Project Online.

```csharp
public sealed class ProjectInfo
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Menginisialisasi instance baru dari kelas `ProjectInfo`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Mendapatkan tanggal dan waktu saat proyek dibuat. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Mendapatkan deskripsi proyek. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Mendapatkan pengidentifikasi unik proyek. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Mendapatkan nilai yang menunjukkan apakah proyek sedang di‑checkout. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Mendapatkan tanggal terbaru saat proyek dipublikasikan. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Mendapatkan tanggal terbaru saat proyek disimpan. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Mendapatkan nama proyek. |

## Contoh

Menampilkan cara membaca informasi tentang proyek dari Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// baca informasi proyek
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


