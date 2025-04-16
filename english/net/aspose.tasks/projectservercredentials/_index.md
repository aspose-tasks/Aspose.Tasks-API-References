---
title: Class ProjectServerCredentials
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectServerCredentials class. Credentials which are used to connect to Project Online or onpremise instance of Project Server
type: docs
weight: 1430
url: /net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Credentials which are used to connect to Project Online or on-premise instance of Project Server.

```csharp
public sealed class ProjectServerCredentials
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Initializes a new instance of the `ProjectServerCredentials` class using URL of Project Web Access endpoint and network credentials. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Initializes a new instance of the `ProjectServerCredentials` class using URL of SharePoint site and valid SPOIDCRL authorization token for SharePoint's PWA (Project Web Access) site. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Initializes a new instance of the `ProjectServerCredentials` class using URL of SharePoint site, user name and password. |

## Properties

| Name | Description |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Gets the authorization token for the SharePoint instance. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Gets the URL of PWA at SharePoint site or URL of on-premise Project Server. For example, https://your_company_name.sharepoint.com/sites/pwa"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Gets the user name for SharePoint site. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Returns a string representation of this instance. |

## Examples

Shows how to use project server credentials to retrieve list of project from Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


