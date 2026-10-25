---
title: "Sınıf ProjectServerCredentials"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectServerCredentials sınıfı. Project Online'a veya Project Server'ın yerel örneğine bağlanmak için kullanılan kimlik bilgileri"
type: docs
weight: 1490
url: /tr/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Project Online veya yerel Project Server örneğine bağlanmak için kullanılan kimlik bilgileri.

```csharp
public sealed class ProjectServerCredentials
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | `ProjectServerCredentials` sınıfının yeni bir örneğini, Project Web Access uç noktasının URL'si ve ağ kimlik bilgilerini kullanarak başlatır. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | `ProjectServerCredentials` sınıfının yeni bir örneğini, SharePoint sitesinin URL'si ve SharePoint'in PWA (Project Web Access) sitesi için geçerli SPOIDCRL yetkilendirme belirteci kullanarak başlatır. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | `ProjectServerCredentials` sınıfının yeni bir örneğini, SharePoint sitesinin URL'si, kullanıcı adı ve şifre kullanarak başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | SharePoint örneği için yetkilendirme belirtecini alır. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | SharePoint sitesindeki PWA'nın URL'sini veya yerel Project Server'ın URL'sini alır. Örneğin, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | SharePoint sitesi için kullanıcı adını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Bu örneğin dize temsili döndürür. |

## Örnekler

Microsoft Project Online'dan proje listesini almak için proje sunucusu kimlik bilgilerinin nasıl kullanılacağını gösterir.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


