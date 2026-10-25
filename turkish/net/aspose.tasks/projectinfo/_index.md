---
title: "Sınıf ProjectInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectInfo sınıfı. Project Online’da mevcut yayınlanmış proje hakkında kısa bilgi."
type: docs
weight: 1470
url: /tr/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Project Online'da bulunan yayınlanmış proje hakkında kısa bilgi.

```csharp
public sealed class ProjectInfo
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectInfo](projectinfo/)() | `ProjectInfo` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Projenin oluşturulduğu tarih ve saati alır. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Projenin açıklamasını alır. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Projenin benzersiz tanımlayıcısını alır. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Projenin çıkış yapılıp yapılmadığını gösteren bir değeri alır. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Projenin yayınlandığı en son tarihi alır. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Projenin kaydedildiği en son tarihi alır. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Projenin adını alır. |

## Örnekler

Project Online’dan projeler hakkında bilgi nasıl okunacağını gösterir.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// projenin bilgilerini oku
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


