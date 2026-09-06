---
title: "类 ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ProjectServerSaveOptions 类。允许在项目保存到 Project Server 或 Project Online 时指定其他选项"
type: docs
weight: 1510
url: /zh/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

允许在将项目保存到 Project Server 或 Project Online 时指定附加选项。

```csharp
public sealed class ProjectServerSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | 初始化 `ProjectServerSaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | 获取或设置队列作业状态请求之间的间隔。默认值为 2 秒。 |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | 获取或设置项目的唯一标识符。应在 Project Server \\ Project Online 实例中唯一。 |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | 获取或设置项目的名称，该名称显示在 Project Server \\ Project Online 项目列表中。应在 Project Server \\ Project Online 实例中唯一。如果省略此值，将使用 Prj.Name 属性的值。 |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | 获取或设置在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。此属性的默认值为 1 分钟。 |

## 示例

展示如何使用 &lt;see cref=\"Aspose.Tasks.ProjectServerSaveOptions\" /&gt; 选项在本地部署的 Project Server 实例中创建新项目。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


