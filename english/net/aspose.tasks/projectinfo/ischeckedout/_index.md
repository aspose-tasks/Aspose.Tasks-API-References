---
title: ProjectInfo.IsCheckedOut
second_title: Aspose.Tasks for .NET API Reference
description: ProjectInfo property. Gets a value indicating whether the project is checked out
type: docs
weight: 50
url: /net/aspose.tasks/projectinfo/ischeckedout/
---
## ProjectInfo.IsCheckedOut property

Gets a value indicating whether the project is checked out.

```csharp
public bool IsCheckedOut { get; }
```

## Examples

Shows how to read information about projects from Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// read project's information
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### See Also

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


