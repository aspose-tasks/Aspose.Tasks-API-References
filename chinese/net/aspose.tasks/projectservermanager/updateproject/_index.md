---
title: "ProjectServerManager.UpdateProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 方法。使用默认保存选项更新 Project ServerProject Online 实例中的现有项目。现有项目将被覆盖。"
type: docs
weight: 70
url: /zh/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

使用默认保存选项在 Project Server\Project Online 实例中更新现有项目。现有项目将被覆盖。

```csharp
public void UpdateProject(Project project)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\\Project Online 实例的项目。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 如果出现通信错误或服务器返回的错误。 |

## 备注

Project 的属性 'project.Get(Prj.Guid)' 应该是存在于 Project Server 帐户 \\ Project Online 实例中的项目的有效 GUID。

## 示例

在此示例中，项目从 Project Online 帐户加载，进行修改后再保存回 Project Online 帐户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

展示如何在 Microsoft Project Online 上更新项目。

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### 另见

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

使用指定的保存选项在 Project Server\Project Online 实例中更新现有项目。现有项目将被覆盖。

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 要保存到 Project Server\\Project Online 实例的项目。 |
| saveOptions | ProjectServerSaveOptions | [`ProjectServerSaveOptions`](../../projectserversaveoptions/) 类的实例。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | 如果出现通信错误或服务器返回的错误。 |

## 备注

saveOptions.ProjectGuid 应设置为存在于 Project Server\\ Project Online 实例中的项目的 GUID。

## 示例

在此示例中，项目从 Project Online 帐户加载，进行修改后再保存回 Project Online 帐户。

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

展示如何在 Microsoft Project Online 上使用 Project Server 保存选项来更新项目。

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### 另见

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


