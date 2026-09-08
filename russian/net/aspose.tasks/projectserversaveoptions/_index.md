---
title: "Класс ProjectServerSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ProjectServerSaveOptions. Позволяет указать дополнительные параметры при сохранении проекта в Project Server или Project Online."
type: docs
weight: 1510
url: /ru/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Позволяет указать дополнительные параметры при сохранении проекта в Project Server или Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Инициализирует новый экземпляр класса `ProjectServerSaveOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Получает или задает интервал между запросами статуса задач очереди. Значение по умолчанию — 2 секунды. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Получает или задает уникальный идентификатор проекта. Должен быть уникальным в пределах экземпляра Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Получает или задает имя проекта, которое отображается в списке проектов Project Server \ Project Online. Должно быть уникальным в пределах экземпляра Project Server \ Project Online. Если значение опущено, вместо него будет использовано значение свойства Prj.Name. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Получает или задает тайм‑аут, используемый при ожидании обработки запроса сохранения проекта службой обработки очереди Project Server. Значение по умолчанию для этого свойства — 1 минута. |

## Примеры

Показывает, как использовать параметры &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; для создания нового проекта в локальном экземпляре Project Server.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


