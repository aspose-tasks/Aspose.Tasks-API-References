---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ProjectServerManager. Инициализирует новый экземпляр класса ProjectServerManager."
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Инициализирует новый экземпляр класса [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| учетные данные | ProjectServerCredentials | Учетные данные, используемые для подключения к учетной записи Project Online. |

## Примеры

В этом примере показано, как создать экземпляр ProjectServerManager для доступа к локальному экземпляру Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

В этом примере показано, как создать экземпляр ProjectServerManager для доступа к учетной записи в сервисе Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Показывает, как прочитать проект из Microsoft Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### См. также

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


