---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerSaveOptions 属性。获取或设置在等待 Project Server 队列处理服务处理保存项目请求时使用的超时时间。此属性的默认值为 1 分钟。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

获取或设置在等待 Project Server 的队列处理服务处理保存项目请求时使用的超时时间。此属性的默认值为 1 分钟。

```csharp
public TimeSpan Timeout { get; set; }
```

## 备注

对于大型项目或 Project Server 实例因响应其他请求而过于繁忙的情况，处理时间可能会更长。

## 示例

展示如何在 Microsoft Project Online 上更新项目并控制保存超时时间。

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


