---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ProjectServerManager 이벤트. 웹 요청이 Project Server의 웹 API로 전송될 때 발생하는 이벤트입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

웹 요청이 Project Server의 웹 API로 전송될 때 발생하는 이벤트입니다.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## 예제

ProjectServerManager.ExecutingWebRequest 이벤트를 사용하여 Project Server에 발행되는 웹 요청을 맞춤 설정하는 방법을 보여줍니다.

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

### 또 보기

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


