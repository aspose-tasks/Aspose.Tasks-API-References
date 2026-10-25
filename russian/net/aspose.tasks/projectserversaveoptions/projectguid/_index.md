---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectServerSaveOptions. Получает или задаёт уникальный идентификатор проекта. Должен быть уникален в пределах экземпляра Project Server Project Online"
type: docs
weight: 30
url: /ru/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

Получает или задает уникальный идентификатор проекта. Должен быть уникальным в пределах экземпляра Project Server \ Project Online.

```csharp
public Guid ProjectGuid { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


