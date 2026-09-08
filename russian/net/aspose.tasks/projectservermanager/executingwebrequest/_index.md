---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Событие ProjectServerManager. Событие, которое вызывается, когда веб‑запрос отправляется в веб‑API Project Server."
type: docs
weight: 20
url: /ru/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Событие, которое вызывается при отправке веб‑запроса к веб‑API Project Server.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Примеры

Показывает, как использовать событие ProjectServerManager.ExecutingWebRequest для настройки веб‑запросов, отправляемых в Project Server.

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

### См. также

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


