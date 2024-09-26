---
title: ProjectServerSaveOptions.ProjectServerSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerSaveOptions constructor. Initializes a new instance of the ProjectServerSaveOptions class
type: docs
weight: 10
url: /net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Initializes a new instance of the [`ProjectServerSaveOptions`](../) class.

```csharp
public ProjectServerSaveOptions()
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


