---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 Project Online 계정 또는 지정된 온프레미스 Project Server 인스턴스에서 프로젝트를 읽고 작업을 수행하는 메서드를 제공하는 클래스입니다. 지원되는 Project Server 버전은 2016 및 2019입니다."
type: docs
weight: 226
url: /ko/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

지정된 Project Online 계정 또는 지정된 온프레미스 Project Server 인스턴스(지원되는 Project Server 버전: 2016 및 2019)에서 프로젝트를 읽고 작업을 수행하는 메서드를 제공하는 클래스입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | 새로운 [ProjectServerManager](../../com.aspose/tasks/projectservermanager) 클래스의 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | 기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Project Server의 웹 API에 웹 요청이 전송될 때 발생하는 이벤트를 가져옵니다. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | 지정된 guid를 가진 프로젝트를 Project Online 계정 \\ Project Server 인스턴스에서 가져옵니다. |
| [getProjectList()](#getProjectList--) | 현재 Project Online 계정 \\ Project Server 인스턴스의 'Working' 저장소에서 프로젝트 목록을 가져옵니다. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | 문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Project Server의 웹 API에 웹 요청이 전송될 때 발생하는 이벤트를 설정합니다. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | 기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 지정된 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


새로운 [ProjectServerManager](../../com.aspose/tasks/projectservermanager) 클래스의 인스턴스를 초기화합니다.

--------------------

&gt; ```
&gt; 이 예제는 온프레미스 Project Server 인스턴스에 액세스하기 위해 ProjectServerManager의 인스턴스를 생성하는 방법을 보여줍니다.
&gt; ``````

 [C#]
string site = \"http://project_server_instance.local/\";
var windowsCredentials = new NetworkCredential(\"Administrator\", \"my_password\", \"DOMAIN\");
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Project Online 계정에 연결하는 데 사용되는 자격 증명입니다. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


기본 저장 옵션을 사용하여 Project Server\\Project Online 인스턴스에 새 프로젝트를 생성합니다.

--------------------

&gt; ```
&gt; 이 예제에서는 프로젝트를 .mpp 파일에서 로드하고 Project Online 계정에 저장합니다.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials(\"https://xxxxxx.sharepoint.com\", \"yyyyy@xxxxxxx.onmicrosoft.com\", \"password\");
var project = new Project(@\"sample.mpp\");
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project Server\Project Online 인스턴스에 저장할 프로젝트. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) 클래스의 인스턴스. |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Project Server의 웹 API에 웹 요청이 전송될 때 발생하는 이벤트를 가져옵니다.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


지정된 guid를 가진 프로젝트를 Project Online 계정 \\ Project Server 인스턴스에서 가져옵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| projectGuid | java.util.UUID | 읽을 프로젝트의 Guid. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


현재 Project Online 계정 \\ Project Server 인스턴스의 'Working' 저장소에서 프로젝트 목록을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - 현재 Project Online 계정 \ Project Server 인스턴스에 있는 프로젝트들의 열거형.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


문제 해결을 위해 프로젝트의 바이너리 데이터를 가져옵니다.

--------------------

&gt; ```
&gt;
&gt; ``````

이 예제에서는 특정 프로젝트에 대한 디버그 정보를 가져옵니다. 결과로 생성된 "debug.zip" 파일을 지원 팀에 전달하여 문제 해결에 사용할 수 있습니다.
 [C#]
var credentials = new ProjectServerCredentials(\"https://xxxxxx.sharepoint.com\", \"yyyyy@xxxxxxx.onmicrosoft.com\", \"password\");
// 가져오려는 프로젝트의 Guid.
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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Project Server\Project Online 인스턴스에 저장할 프로젝트. |

--------------------

Project의 속성 'project.Get(Prj.Guid)'은 Project Server 계정 \ Project Online 인스턴스에 존재하는 프로젝트의 유효한 guid이어야 합니다. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


지정된 저장 옵션을 사용하여 Project Server\Project Online 인스턴스의 기존 프로젝트를 업데이트합니다. 기존 프로젝트는 덮어쓰게 됩니다.

--------------------

&gt; ```
&gt; 이 예제에서는 프로젝트를 Project Online 계정에서 로드하고 수정한 뒤 다시 Project Online 계정에 저장합니다.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials(\"https://xxxxxx.sharepoint.com\", \"yyyyy@xxxxxxx.onmicrosoft.com\", \"password\");
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

