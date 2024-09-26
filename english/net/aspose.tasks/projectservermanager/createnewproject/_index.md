---
title: ProjectServerManager.CreateNewProject
second_title: Aspose.Tasks for .NET API Reference
description: ProjectServerManager method. Creates new project in Project ServerProject Online instance using default save options
type: docs
weight: 30
url: /net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Creates new project in Project Server\Project Online instance using default save options.

```csharp
public void CreateNewProject(Project project)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | The project to save to Project Server\Project Online instance. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In case of communication error or error returned by a server. |

## Examples

In this example the project is loaded from .mpp file and saved to Project Online account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Shows how to use ProjectServerManager to create a new project on Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Creates new project in Project Server\Project Online instance using the specified save options.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | The project to save to Project Server\Project Online instance. |
| saveOptions | ProjectServerSaveOptions | Instance of [`ProjectServerSaveOptions`](../../projectserversaveoptions/) class. |

### Exceptions

| exception | condition |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | In case of communication error or error returned by a server. |

## Examples

In this example the project is loaded from .mpp file and saved to Project Online account.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


