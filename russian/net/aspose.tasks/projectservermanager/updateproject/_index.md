---
title: "ProjectServerManager.UpdateProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectServerManager. Обновляет существующий проект в экземпляре Project Server\\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан"
type: docs
weight: 70
url: /ru/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Обновляет существующий проект в экземпляре Project Server\Project Online, используя параметры сохранения по умолчанию. Существующий проект будет перезаписан.

```csharp
public void UpdateProject(Project project)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект для сохранения в экземпляр Project Server\Project Online. |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

## Примечания

Свойство проекта 'project.Get(Prj.Guid)' должно быть действительным GUID проекта, который существует в учетной записи Project Server \ Project Online.

## Примеры

В этом примере проект загружается из учетной записи Project Online, изменяется и сохраняется обратно в учетную запись Project Online.

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

Показывает, как обновить проект в Microsoft Project Online.

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

### См. также

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Обновляет существующий проект в экземпляре Project Server\Project Online, используя указанные параметры сохранения. Существующий проект будет перезаписан.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| проект | Project | Проект для сохранения в экземпляр Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Экземпляр класса [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Исключения

| исключение | условие |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | В случае ошибки связи или ошибки, возвращенной сервером. |

## Примечания

saveOptions.ProjectGuid должен быть установлен в GUID проекта, который существует в экземпляре Project Server\Project Online.

## Примеры

В этом примере проект загружается из учетной записи Project Online, изменяется и сохраняется обратно в учетную запись Project Online.

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

Показывает, как обновить проект в Microsoft Project Online с использованием параметров сохранения Project Server.

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

### См. также

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


