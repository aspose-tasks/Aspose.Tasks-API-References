---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerSaveOptions 构造函数。初始化 ProjectServerSaveOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

初始化 [`ProjectServerSaveOptions`](../) 类的新实例。

```csharp
public ProjectServerSaveOptions()
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


