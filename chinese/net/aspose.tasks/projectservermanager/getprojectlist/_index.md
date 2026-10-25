---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 方法。从当前 Project Online 账户的工作存储中获取项目列表 Project Server 实例。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

从当前 Project Online 帐户\Project Server 实例的 “Working” 存储中获取项目列表。

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### 返回值

当前 Project Online 账户 \ Project Server 实例中的项目枚举。

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


