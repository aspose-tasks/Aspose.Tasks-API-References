---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ProjectServerSaveOptions. Инициализирует новый экземпляр класса ProjectServerSaveOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Инициализирует новый экземпляр класса [`ProjectServerSaveOptions`](../)

```csharp
public ProjectServerSaveOptions()
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


