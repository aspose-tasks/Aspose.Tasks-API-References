---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API 参考"
description: "提供读取和对指定 Project Online 帐户或指定本地 Project Server 实例中的项目执行操作的方法的类。支持 Project Server 2016 和 2019 版本。"
type: docs
weight: 226
url: /zh/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

该类提供在指定的 Project Online 帐户或指定的本地 Project Server 实例中读取项目并执行操作的方法（支持 Project Server 2016 和 2019 版本）。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | 初始化一个新的 [ProjectServerManager](../../com.aspose/tasks/projectservermanager) 类的实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | 使用默认保存选项在 Project Server\\Project Online 实例中创建新项目。 |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 使用指定的保存选项在 Project Server\\Project Online 实例中创建新项目。 |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | 获取在向 Project Server 的 Web API 发送网络请求时触发的事件。 |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | 从 Project Online 帐户 \\ Project Server 实例中获取具有指定 GUID 的项目。 |
| [getProjectList()](#getProjectList--) | 从当前 Project Online 帐户 \\ Project Server 实例的 'Working' 存储中获取项目列表。 |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | 获取项目的二进制数据以用于故障排除。 |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | 设置在向 Project Server 的 Web API 发送网络请求时触发的事件。 |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | 使用默认保存选项在 Project Server\\Project Online 实例中更新现有项目。 |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 使用指定的保存选项在 Project Server\\Project Online 实例中更新现有项目。 |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


初始化一个新的 [ProjectServerManager](../../com.aspose/tasks/projectservermanager) 类的实例。

--------------------

&gt; ```
&gt; 本示例展示了如何创建 ProjectServerManager 实例以访问本地 Project Server 实例。
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | 用于连接到 Project Online 帐户的凭据。 |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


使用默认保存选项在 Project Server\\Project Online 实例中创建新项目。

--------------------

&gt; ```
&gt; 在本示例中，项目从 .mpp 文件加载并保存到 Project Online 帐户。
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 要保存到 Project Server\\Project Online 实例的项目。 |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 类的实例。 |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


获取在向 Project Server 的 Web API 发送网络请求时触发的事件。

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


从 Project Online 帐户 \\ Project Server 实例中获取具有指定 GUID 的项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectGuid | java.util.UUID | 要读取的项目的 Guid。 |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


从当前 Project Online 帐户 \\ Project Server 实例的 'Working' 存储中获取项目列表。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - 当前 Project Online 帐户 \\ Project Server 实例中的项目枚举。
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


获取项目的二进制数据以用于故障排除。

--------------------

&gt; ```
&gt;
&gt; ``````

在此示例中，检索到特定项目的调试信息。您可以将生成的 \"debug.zip\" 发送给支持团队以进行故障排除。
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// 正在尝试获取的项目 Guid。
var projectGuid = new Guid(\"e0294bfb-5657-45c8-9cc5-82169fb95d69\");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@\"c:\\debug.zip\"))
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | 要保存到 Project Server\\Project Online 实例的项目。 |

--------------------

Project 的属性 'project.Get(Prj.Guid)' 应该是存在于 Project Server 帐户 \\ Project Online 实例中的项目的有效 guid。 |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


使用指定的保存选项更新 Project Server\\Project Online 实例中的现有项目。现有项目将被覆盖。

--------------------

&gt; ```
&gt; 在此示例中，项目从 Project Online 帐户加载，进行修改后再保存回 Project Online 帐户。
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add(\"New task\");
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

