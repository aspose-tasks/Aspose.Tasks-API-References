---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectServerSaveOptions. Получает или задаёт интервал между запросами статуса задач в очереди. Значение по умолчанию — 2 секунды"
type: docs
weight: 20
url: /ru/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

Получает или задает интервал между запросами статуса задач очереди. Значение по умолчанию — 2 секунды.

```csharp
public TimeSpan PollingInterval { get; set; }
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


