---
title: "Sınıf ProjectServerManager"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ProjectServerManager sınıfı. Belirtilen Project Online hesabındaki veya belirtilen yerel Project Server örneğindeki projeleri okuma ve işlemler gerçekleştirme yöntemlerini sağlayan sınıf. Project Server sürümleri 2016 ve 2019 desteklenir."
type: docs
weight: 1500
url: /tr/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

Belirtilen Project Online hesabındaki veya belirtilen yerel Project Server örneğindeki projeleri okumak ve işlemler gerçekleştirmek için yöntemler sağlayan sınıf (Project Server'ın 2016 ve 2019 sürümleri desteklenir).

```csharp
public sealed class ProjectServerManager
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | `ProjectServerManager` sınıfının yeni bir örneğini başlatır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Varsayılan kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğinde yeni proje oluşturur. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğinde yeni bir proje oluşturur. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Project Online hesabı \\ Project Server örneğinden belirtilen guid'e sahip projeyi alır. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Mevcut Project Online hesabı \\ Project Server örneğinin 'Working' deposundan proje listesini alır. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Sorun giderme amaçları için projenin ikili verilerini alır. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Varsayılan kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğindeki mevcut projeyi günceller. Mevcut proje üzerine yazılacak. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Belirtilen kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğindeki mevcut projeyi günceller. Mevcut proje üzerine yazılacak. |

## Olaylar

| Ad | Açıklama |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olay. |

## Örnekler

Microsoft Project Online'da önceden tanımlı kaydetme seçenekleriyle yeni bir proje oluşturmak için Project Server yöneticisinin nasıl kullanılacağını gösterir.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


