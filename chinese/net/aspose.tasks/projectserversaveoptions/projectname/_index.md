---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerSaveOptions 属性。获取或设置项目的名称，该名称显示在 Project Server / Project Online 项目列表中。应在 Project Server / Project Online 实例中唯一。如果省略该值，将使用 Prj.Name 属性的值。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

获取或设置项目的名称，该名称显示在 Project Server \\ Project Online 项目列表中。应在 Project Server \\ Project Online 实例中唯一。如果省略此值，将使用 Prj.Name 属性的值。

```csharp
public string ProjectName { get; set; }
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


