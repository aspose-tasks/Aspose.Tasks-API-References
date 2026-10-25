---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectServerManager olayı. Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olay."
type: docs
weight: 20
url: /tr/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olay.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Örnekler

ProjectServerManager.ExecutingWebRequest olayını, Project Server'a gönderilen web isteklerini özelleştirmek için nasıl kullanacağınızı gösterir.

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

### Ayrıca Bakınız

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


