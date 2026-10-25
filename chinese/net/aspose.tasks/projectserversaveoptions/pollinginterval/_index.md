---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerSaveOptions 属性。获取或设置队列作业状态请求之间的间隔。默认值为 2 秒"
type: docs
weight: 20
url: /zh/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

获取或设置队列作业状态请求之间的间隔。默认值为 2 秒。

```csharp
public TimeSpan PollingInterval { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


