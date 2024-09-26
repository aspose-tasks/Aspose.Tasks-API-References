---
title: ProjectServerSaveOptions.ProjectName
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerSaveOptions property. Gets or sets name of a project which is displayed in Project Server  Project Online projects list. Should be unique within Project Server  Project Online instance. Is the value is omitted the value of Prj.Name property will be used instead
type: docs
weight: 40
url: /net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Gets or sets name of a project which is displayed in Project Server \ Project Online projects list. Should be unique within Project Server \ Project Online instance. Is the value is omitted, the value of Prj.Name property will be used instead.

```csharp
public string ProjectName { get; set; }
```

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

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


