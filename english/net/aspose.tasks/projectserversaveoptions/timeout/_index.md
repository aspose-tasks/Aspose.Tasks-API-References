---
title: ProjectServerSaveOptions.Timeout
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerSaveOptions property. Gets or sets timeout used when waiting for processing of save project request by a Project Servers queue processing service. The default value for this property is 1 minute
type: docs
weight: 50
url: /net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Gets or sets timeout used when waiting for processing of save project request by a Project Server's queue processing service. The default value for this property is 1 minute.

```csharp
public TimeSpan Timeout { get; set; }
```

## Remarks

The processing time may be longer for large projects or in case when Project Server instance is too busy responding to other requests.

## Examples

Shows how to update project on Microsoft Project Online and control save timeout value.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### See Also

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


