---
title: ProjectServerManager.GetProject
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager method. Gets the project with the specified guid from the Project Online account  Project Server instance
type: docs
weight: 40
url: /net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Gets the project with the specified guid from the Project Online account \ Project Server instance.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| projectGuid | Guid | The Guid of the project to read. |

### Return Value

Instance of [`Project`](../../project/) class which represents project read from Project Online \ Project Server.

## Examples

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


