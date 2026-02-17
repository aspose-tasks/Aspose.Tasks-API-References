---
title: Class ProjectServerManager
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectServerManager class. The class which provides the methods to read and to perform operations on projects in the specified Project Online account or in the specified onpremise Project Server instance Project Servers versions 2016 and 2019 are supported
type: docs
weight: 1480
url: /net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

The class which provides the methods to read and to perform operations on projects in the specified Project Online account or in the specified on-premise Project Server instance (Project Server's versions 2016 and 2019 are supported).

```csharp
public sealed class ProjectServerManager
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Initializes a new instance of the `ProjectServerManager` class. |

## Methods

| Name | Description |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Creates new project in Project Server\Project Online instance using default save options. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Creates new project in Project Server\Project Online instance using the specified save options. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Gets the project with the specified guid from the Project Online account \ Project Server instance. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Gets the list of projects from 'Working' store of the current Project Online account \ Project Server instance. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Gets the project's binary data for troubleshooting purposes. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Updates existing project in Project Server\Project Online instance using default save options. The existing project will be overwritten. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Updates existing project in Project Server\Project Online instance using the specified save options. The existing project will be overwritten. |

## Events

| Name | Description |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | An event that is raised when the web request is sent to Project Server's web API. |

## Examples

Shows how to use Project Server manager to create a new project with predefined save options on Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


