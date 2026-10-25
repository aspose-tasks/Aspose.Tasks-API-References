---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectServerSaveOptions. Получает или задаёт тайм‑аут, используемый при ожидании обработки запроса сохранения проекта службой обработки очереди Project Servers. Значение по умолчанию для этого свойства — 1 минута"
type: docs
weight: 50
url: /ru/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Получает или задает тайм‑аут, используемый при ожидании обработки запроса сохранения проекта службой обработки очереди Project Server. Значение по умолчанию для этого свойства — 1 минута.

```csharp
public TimeSpan Timeout { get; set; }
```

## Примечания

Время обработки может быть дольше для крупных проектов или в случае, когда экземпляр Project Server слишком занят обработкой других запросов.

## Примеры

Показывает, как обновить проект в Microsoft Project Online и управлять значением тайм‑аута сохранения.

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


