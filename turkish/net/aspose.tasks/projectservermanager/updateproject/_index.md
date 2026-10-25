---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager yöntemi. Varsayılan kaydetme seçeneklerini kullanarak Project ServerProject Online örneğinde mevcut projeyi günceller. Mevcut proje üzerine yazılacak."
type: docs
weight: 70
url: /tr/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Varsayılan kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğindeki mevcut projeyi günceller. Mevcut proje üzerine yazılacak.

```csharp
public void UpdateProject(Project project)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Project Server\\Project Online örneğine kaydedilecek proje. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya sunucu tarafından döndürülen hata durumunda. |

## Açıklamalar

Projenin 'project.Get(Prj.Guid)' özelliği, Project Server hesabı \\ Project Online örneğinde mevcut olan bir projenin geçerli guid'i olmalıdır.

## Örnekler

Bu örnekte proje, Project Online hesabından yüklenir, değiştirilir ve tekrar Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Microsoft Project Online'da projenin nasıl güncelleneceğini gösterir.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Belirtilen kaydetme seçeneklerini kullanarak Project Server\\Project Online örneğindeki mevcut projeyi günceller. Mevcut proje üzerine yazılacak.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | Project | Project Server\\Project Online örneğine kaydedilecek proje. |
| saveOptions | ProjectServerSaveOptions | Sınıfının bir örneği [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### İstisnalar

| istisna | koşul |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | İletişim hatası veya sunucu tarafından döndürülen hata durumunda. |

## Açıklamalar

saveOptions.ProjectGuid, Project Server\\ Project Online örneğinde mevcut olan bir projenin guid'ine ayarlanmalıdır.

## Örnekler

Bu örnekte proje, Project Online hesabından yüklenir, değiştirilir ve tekrar Project Online hesabına kaydedilir.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Project Server kaydetme seçeneklerinin kullanımıyla Microsoft Project Online'da projenin nasıl güncelleneceğini gösterir.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Ayrıca Bakınız

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


