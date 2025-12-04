---
title: ProjectServerManager
second_title: Aspose.Tasks for Java API Reference
description: The class which provides the methods to read and to perform operations on projects in the specified Project Online account or in the specified on-premise Project Server instance Project Servers versions 2016 and 2019 are supported.
type: docs
weight: 225
url: /java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

The class which provides the methods to read and to perform operations on projects in the specified Project Online account or in the specified on-premise Project Server instance (Project Server's versions 2016 and 2019 are supported).
## Constructors

| Constructor | Description |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Initializes a new instance of the [ProjectServerManager](../../com.aspose.tasks/projectservermanager) class. |
## Methods

| Method | Description |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Creates new project in Project Server\\Project Online instance using default save options. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Creates new project in Project Server\\Project Online instance using the specified save options. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Gets an event that is raised when the web request is sent to Project Server's web API. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Gets the project with the specified guid from the Project Online account \\ Project Server instance. |
| [getProjectList()](#getProjectList--) | Gets the list of projects from 'Working' store of the current Project Online account \\ Project Server instance. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Gets the project's binary data for troubleshooting purposes. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Sets an event that is raised when the web request is sent to Project Server's web API. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Updates existing project in Project Server\\Project Online instance using default save options. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Updates existing project in Project Server\\Project Online instance using the specified save options. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Initializes a new instance of the [ProjectServerManager](../../com.aspose.tasks/projectservermanager) class.

--------------------

&gt; ```
&gt; This example shows how to create instance of ProjectServerManager to access on-premise instance of Project Server.
&gt; ``````

 [C#]
 string site = "http://project_server_instance.local/";
 var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
 var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
 ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
 
```

--------------------

&gt; ```
&gt; This example shows how to create instance of ProjectServerManager to access account in Project Online service.
&gt; ``````

 [C#]
 var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
 ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Credentials used to connect to Project Online account. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Creates new project in Project Server\\Project Online instance using default save options.

--------------------

&gt; ```
&gt; In this example the project is loaded from .mpp file and saved to Project Online account.
&gt; ``````

 [C#]
 var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
 var project = new Project(@"sample.mpp");
 ProjectServerManager manager = new ProjectServerManager(credentials);
 manager.CreateNewProject(project);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | The project to save to Project Server\\Project Online instance. |

### createNewProject(Project project, ProjectServerSaveOptions saveOptions) {#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void createNewProject(Project project, ProjectServerSaveOptions saveOptions)
```


Creates new project in Project Server\\Project Online instance using the specified save options.

--------------------

&gt; ```
&gt; In this example the project is loaded from .mpp file and saved to Project Online account.
&gt; ``````

 [C#]
 var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
 var project = new Project(@"sample.mpp");
 ProjectServerManager manager = new ProjectServerManager(credentials);
 manager.CreateNewProject(project, new ProjectServerSaveOptions
 {
     ProjectName = "My new project"
 });
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | The project to save to Project Server\\Project Online instance. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instance of [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) class. |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Gets an event that is raised when the web request is sent to Project Server's web API.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Gets the project with the specified guid from the Project Online account \\ Project Server instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectGuid | java.util.UUID | The Guid of the project to read. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Gets the list of projects from 'Working' store of the current Project Online account \\ Project Server instance.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - An enumeration of projects in the current Project Online account \\ Project Server instance.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Gets the project's binary data for troubleshooting purposes.

--------------------

&gt; ```
&gt; 
&gt; ``````

 In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
 [C#]
 var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
 // Guid of project you are trying to get.
 var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
 ProjectServerManager manager = new ProjectServerManager(credentials);
 using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
 {
     using (var stream = manager.GetProjectRawData(projectGuid))
     {
         stream.CopyTo(fileStream);
     }
 }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectGuid | java.util.UUID | The Guid of the project to read. |

**Returns:**
java.io.InputStream - Stream containing raw project's data.
### setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value) {#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--}
```
public final void setExecutingWebRequest(Event<WebRequestEventArgs> value)
```


Sets an event that is raised when the web request is sent to Project Server's web API.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.tasks.Event&lt;com.aspose.tasks.WebRequestEventArgs&gt; | an event that is raised when the web request is sent to Project Server's web API. |

### updateProject(Project project) {#updateProject-com.aspose.tasks.Project-}
```
public final void updateProject(Project project)
```


Updates existing project in Project Server\\Project Online instance using default save options. The existing project will be overwritten.

--------------------

&gt; ```
&gt; In this example the project is loaded from Project Online account, modified and saved back to Project Online account.
&gt; ``````

 [C#]
 var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
 ProjectServerManager manager = new ProjectServerManager(credentials);
 var projectList = manager.GetProjectList();
 var projectGuid = projectList.First().Id;
 var project = manager.GetProject(projectGuid);
 var task = project.RootTask.Children.Add("New task");
 manager.UpdateProject(project);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | The project to save to Project Server\\Project Online instance.

--------------------

Project's property 'project.Get(Prj.Guid)' should be a valid guid of a project which exists in Project Server account \\ Project Online instance. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Updates existing project in Project Server\\Project Online instance using the specified save options. The existing project will be overwritten.

--------------------

&gt; ```
&gt; In this example the project is loaded from Project Online account, modified and saved back to Project Online account.
&gt; ``````

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



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | The project to save to Project Server\\Project Online instance. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instance of [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) class.

--------------------

saveOptions.ProjectGuid should be set to a guid of a project which exists on Project Server\\ Project Online instance. |

