---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yapıcı. ProjectServerManager sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

[`ProjectServerManager`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kimlik bilgileri | ProjectServerCredentials | Project Online hesabına bağlanmak için kullanılan kimlik bilgileri. |

## Örnekler

Bu örnek, Project Server'ın yerel örneğine erişmek için ProjectServerManager örneği oluşturmayı gösterir.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Bu örnek, Project Online hizmetindeki hesaba erişmek için ProjectServerManager örneği oluşturmayı gösterir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

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

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


