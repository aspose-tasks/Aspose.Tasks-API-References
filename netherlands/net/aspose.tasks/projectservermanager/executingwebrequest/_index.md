---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager‑event. Een gebeurtenis die wordt geactiveerd wanneer het webverzoek naar de web‑API van Project Server wordt verzonden."
type: docs
weight: 20
url: /nl/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

Een gebeurtenis die wordt opgehaald wanneer het webverzoek naar de web‑API van Project Server wordt verzonden.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## Voorbeelden

Toont hoe het ProjectServerManager.ExecutingWebRequest‑event te gebruiken om webverzoeken die naar Project Server worden gestuurd aan te passen.

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

### Zie ook

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


