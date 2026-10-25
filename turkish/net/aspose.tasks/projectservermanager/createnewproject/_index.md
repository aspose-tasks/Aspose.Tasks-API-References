---
title: "ProjectServerManager.CreateNewProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yöntemi. Varsayılan kaydetme seçeneklerini kullanarak Project ServerProject Online örneğinde yeni proje oluşturur"
type: docs
weight: 30
url: /tr/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Varsayılan kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğinde yeni proje oluşturur.

```csharp
public void CreateNewProject(Project project)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Project Server\\Project Online örneğine kaydedilecek proje. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya sunucu tarafından döndürülen hata durumunda. |

## Örnekler

Bu örnekte proje .mpp dosyasından yüklenir ve Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Microsoft Project Online'da yeni bir proje oluşturmak için ProjectServerManager kullanımını gösterir.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Belirtilen kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğinde yeni bir proje oluşturur.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Project Server\\Project Online örneğine kaydedilecek proje. |
| saveOptions | ProjectServerSaveOptions | Sınıfının bir örneği [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### İstisnalar

| istisna | koşul |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya sunucu tarafından döndürülen hata durumunda. |

## Örnekler

Bu örnekte proje .mpp dosyasından yüklenir ve Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


