---
title: "ProjectInfo.LastPublishedDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectInfo. Mendapatkan tanggal terbaru saat proyek dipublikasikan"
type: docs
weight: 60
url: /id/net/aspose.tasks/projectinfo/lastpublisheddate/
---
## ProjectInfo.LastPublishedDate property

Mendapatkan tanggal terbaru saat proyek dipublikasikan.

```csharp
public DateTime LastPublishedDate { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


