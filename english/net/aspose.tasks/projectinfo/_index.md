---
title: Class ProjectInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectInfo class. Brief info about the published project available on Project Online
type: docs
weight: 1450
url: /net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Brief info about the published project available on Project Online.

```csharp
public sealed class ProjectInfo
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Initializes a new instance of the `ProjectInfo` class. |

## Properties

| Name | Description |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Gets the date and time when the project was created. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Gets the description of the project. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Gets the unique identifier of the project. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Gets a value indicating whether the project is checked out. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Gets the most recent date when the project was published. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Gets the most recent date when the project was saved. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Gets the name of the project. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


