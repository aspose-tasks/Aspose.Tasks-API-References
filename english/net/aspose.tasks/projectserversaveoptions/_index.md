---
title: Class ProjectServerSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProjectServerSaveOptions class. Allows to specify additional options when project is saved to Project Server or Project Online
type: docs
weight: 1480
url: /net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Allows to specify additional options when project is saved to Project Server or Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Initializes a new instance of the `ProjectServerSaveOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Gets or sets interval between queue job status requests. The default value is 2 seconds. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Gets or sets unique identifier of a project. Should be unique within Project Server \ Project Online instance. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Gets or sets name of a project which is displayed in Project Server \ Project Online projects list. Should be unique within Project Server \ Project Online instance. Is the value is omitted, the value of Prj.Name property will be used instead. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Gets or sets timeout used when waiting for processing of save project request by a Project Server's queue processing service. The default value for this property is 1 minute. |

## Examples

Shows how to use &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; options to create a new project in on-premise instance of Project Server.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
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


