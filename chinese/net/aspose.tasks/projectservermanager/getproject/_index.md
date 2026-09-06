---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 方法。 从 Project Online 帐户的 Project Server 实例获取具有指定 guid 的项目"
type: docs
weight: 40
url: /zh/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

从 Project Online 帐户\Project Server 实例中获取具有指定 guid 的项目。

```csharp
public Project GetProject(Guid projectGuid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectGuid | Guid | 要读取的项目的 Guid。 |

### 返回值

`[`Project`](../../project/)` 类的实例，表示从 Project Online \\ Project Server 读取的项目。

## 示例

展示如何从 Microsoft Project Online 读取项目。

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

### 另见

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


