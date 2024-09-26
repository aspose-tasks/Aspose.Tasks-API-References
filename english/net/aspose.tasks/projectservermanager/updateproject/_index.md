---
title: ProjectServerManager.UpdateProject
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager method. Updates existing project in Project ServerProject Online instance using default save options. The existing project will be overwritten
type: docs
weight: 70
url: /net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Updates existing project in Project Server\Project Online instance using default save options. The existing project will be overwritten.

```csharp
public void UpdateProject(Project project)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | The project to save to Project Server\Project Online instance. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In case of communication error or error returned by a server. |

## Remarks

Project's property 'project.Get(Prj.Guid)' should be a valid guid of a project which exists in Project Server account \ Project Online instance.

## Examples

In this example the project is loaded from Project Online account, modified and saved back to Project Online account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Shows how to update project on Microsoft Project Online.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

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

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### See Also

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Updates existing project in Project Server\Project Online instance using the specified save options. The existing project will be overwritten.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | The project to save to Project Server\Project Online instance. |
| saveOptions | ProjectServerSaveOptions | Instance of [`ProjectServerSaveOptions`](../../projectserversaveoptions/) class. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In case of communication error or error returned by a server. |

## Remarks

saveOptions.ProjectGuid should be set to a guid of a project which exists on Project Server\ Project Online instance.

## Examples

In this example the project is loaded from Project Online account, modified and saved back to Project Online account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Shows how to update project on Microsoft Project Online with an usage of Project Server save options.

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


