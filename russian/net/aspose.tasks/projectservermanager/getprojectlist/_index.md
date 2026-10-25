---
title: "ProjectServerManager.GetProjectList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectServerManager. Получает список проектов из рабочего хранилища текущей учетной записи Project Online экземпляра Project Server."
type: docs
weight: 50
url: /ru/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Получает список проектов из хранилища 'Working' текущей учетной записи Project Online \ экземпляра Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Возвращаемое значение

Перечисление проектов в текущей учетной записи Project Online \ экземпляре Project Server.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


