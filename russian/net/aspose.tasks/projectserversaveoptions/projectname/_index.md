---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectServerSaveOptions. Получает или задаёт имя проекта, отображаемое в списке проектов Project Server Project Online. Должно быть уникальным в пределах экземпляра Project Server Project Online. Если значение опущено, будет использовано значение свойства Prj.Name"
type: docs
weight: 40
url: /ru/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Получает или задает имя проекта, которое отображается в списке проектов Project Server \ Project Online. Должно быть уникальным в пределах экземпляра Project Server \ Project Online. Если значение опущено, вместо него будет использовано значение свойства Prj.Name.

```csharp
public string ProjectName { get; set; }
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


