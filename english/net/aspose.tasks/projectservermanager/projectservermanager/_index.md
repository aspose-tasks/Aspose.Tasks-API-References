---
title: ProjectServerManager.ProjectServerManager
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager constructor. Initializes a new instance of the ProjectServerManager class
type: docs
weight: 10
url: /net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Initializes a new instance of the [`ProjectServerManager`](../) class.

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parameter | Type | Description |
| --- | --- | --- |
| credentials | ProjectServerCredentials | Credentials used to connect to Project Online account. |

## Examples

This example shows how to create instance of ProjectServerManager to access on-premise instance of Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

This example shows how to create instance of ProjectServerManager to access account in Project Online service.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Shows how to read a project from Microsoft Project Online.

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

### See Also

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


