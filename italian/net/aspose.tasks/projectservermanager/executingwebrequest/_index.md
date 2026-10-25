---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Evento ProjectServerManager. Un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server."
type: docs
weight: 20
url: /it/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Esempi

Mostra come utilizzare l'evento ProjectServerManager.ExecutingWebRequest per personalizzare le richieste web inviate a Project Server.

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

### Vedi anche

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


