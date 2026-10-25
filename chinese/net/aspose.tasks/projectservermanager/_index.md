---
title: "类 ProjectServerManager"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectServerManager 类。该类提供读取和对指定的 Project Online 帐户或指定的本地部署 Project Server 实例中的项目执行操作的方法。支持的 Project Server 版本为 2016 和 2019。"
type: docs
weight: 1500
url: /zh/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

该类提供在指定的 Project Online 帐户或指定的本地 Project Server 实例（支持 Project Server 2016 和 2019 版本）中读取和执行项目操作的方法。

```csharp
public sealed class ProjectServerManager
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | 初始化 `ProjectServerManager` 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | 使用默认保存选项在 Project Server\\Project Online 实例中创建新项目。 |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | 使用指定的保存选项在 Project Server\Project Online 实例中创建新项目。 |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | 从 Project Online 帐户\Project Server 实例中获取具有指定 guid 的项目。 |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | 从当前 Project Online 帐户\Project Server 实例的 “Working” 存储中获取项目列表。 |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | 获取项目的二进制数据以用于故障排除。 |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | 使用默认保存选项在 Project Server\Project Online 实例中更新现有项目。现有项目将被覆盖。 |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | 使用指定的保存选项在 Project Server\Project Online 实例中更新现有项目。现有项目将被覆盖。 |

## 事件

| 名称 | 描述 |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | 当向 Project Server 的 Web API 发送网络请求时触发的事件。 |

## 示例

展示如何使用 Project Server 管理器在 Microsoft Project Online 上使用预定义的保存选项创建新项目。

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


