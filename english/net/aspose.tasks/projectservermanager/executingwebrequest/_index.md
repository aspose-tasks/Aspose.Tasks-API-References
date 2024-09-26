---
title: ProjectServerManager.ExecutingWebRequest
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager event. An event that is raised when the web request is sent to Project Servers web API
type: docs
weight: 20
url: /net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

An event that is raised when the web request is sent to Project Server's web API.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Examples

Shows how to use ProjectServerManager.ExecutingWebRequest event to customize web requests issued to Project Server.

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

### See Also

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


