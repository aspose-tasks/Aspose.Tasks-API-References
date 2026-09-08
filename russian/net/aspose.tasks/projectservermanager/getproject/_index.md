---
title: "ProjectServerManager.GetProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectServerManager. Получает проект с указанным guid из аккаунта Project Online и экземпляра Project Server"
type: docs
weight: 40
url: /ru/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Получает проект с указанным GUID из учетной записи Project Online \ экземпляра Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| projectGuid | Guid | Guid проекта, который нужно прочитать. |

### Возвращаемое значение

Экземпляр класса [`Project`](../../project/), представляющий проект, прочитанный из Project Online \\ Project Server.

## Примеры

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


