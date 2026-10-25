---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectServerManager‑constructor. Initialiseert een nieuwe instantie van de ProjectServerManager‑klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Initialiseert een nieuwe instantie van de [`ProjectServerManager`](../)‑klasse.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| referenties | ProjectServerCredentials | Referenties die worden gebruikt om verbinding te maken met een Project Online‑account. |

## Voorbeelden

Dit voorbeeld toont hoe een instantie van ProjectServerManager te maken om toegang te krijgen tot een on-premise instantie van Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Dit voorbeeld toont hoe een instantie van ProjectServerManager te maken om toegang te krijgen tot een account in de Project Online-service.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Toont hoe een project te lezen van Microsoft Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### Zie ook

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


