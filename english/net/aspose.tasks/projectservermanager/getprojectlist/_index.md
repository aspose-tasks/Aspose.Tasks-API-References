---
title: ProjectServerManager.GetProjectList
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager method. Gets the list of projects from Working store of the current Project Online account  Project Server instance
type: docs
weight: 50
url: /net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Gets the list of projects from 'Working' store of the current Project Online account \ Project Server instance.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Return Value

An enumeration of projects in the current Project Online account \ Project Server instance.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


