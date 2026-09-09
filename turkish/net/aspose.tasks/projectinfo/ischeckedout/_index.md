---
title: "ProjectInfo.IsCheckedOut"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectInfo özelliği. Projenin çıkış yapılıp yapılmadığını gösteren bir değer alır"
type: docs
weight: 50
url: /tr/net/aspose.tasks/projectinfo/ischeckedout/
---
## ProjectInfo.IsCheckedOut property

Projenin çıkış yapılıp yapılmadığını gösteren bir değeri alır.

```csharp
public bool IsCheckedOut { get; }
```

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

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


