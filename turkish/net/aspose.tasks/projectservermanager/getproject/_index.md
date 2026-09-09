---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yöntemi. Belirtilen guid'e sahip projeyi Project Online hesabından Project Server örneğinden alır"
type: docs
weight: 40
url: /tr/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Project Online hesabı \\ Project Server örneğinden belirtilen guid'e sahip projeyi alır.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectGuid | Guid | Okunacak projenin Guid'i. |

### Dönüş Değeri

Project Online \ Project Server'dan okunan projeyi temsil eden [`Project`](../../project/) sınıfının bir örneği.

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


