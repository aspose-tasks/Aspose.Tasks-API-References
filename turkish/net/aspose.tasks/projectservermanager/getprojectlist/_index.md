---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yöntemi. Mevcut Project Online hesabının Çalışma deposundan Project Server örneği projelerinin listesini alır"
type: docs
weight: 50
url: /tr/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Mevcut Project Online hesabı \\ Project Server örneğinin 'Working' deposundan proje listesini alır.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Dönüş Değeri

Mevcut Project Online hesabı \ Project Server örneğindeki projelerin bir numaralandırması.

## Örnekler

Microsoft Project Online'dan bir projenin nasıl okunacağını gösterir.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### Ayrıca Bakınız

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


