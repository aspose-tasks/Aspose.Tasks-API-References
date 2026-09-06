---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ProjectServerManager 事件。当向 Project Server 的 Web API 发送请求时触发的事件。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

当向 Project Server 的 Web API 发送网络请求时触发的事件。

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## 示例

展示如何使用 ProjectServerManager.ExecutingWebRequest 事件来自定义发送到 Project Server 的 Web 请求。

```csharp
try
{
    const string SiteUrl = "https://myprojectserver/sites/pwa";
    const string UserName = "test_user";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SiteUrl, new NetworkCredential(UserName, Password));

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.ExecutingWebRequest += delegate (object sender, WebRequestEventArgs e)
    {
        e.WebRequest.Headers.Add("XMyCustomHeader", "testvalue");
    };

    var list = manager.GetProjectList();
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另见

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


