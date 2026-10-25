---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定された Project Online アカウントまたは指定されたオンプレミスの Project Server インスタンス上のプロジェクトを読み取り、操作するメソッドを提供するクラスです。サポートされている Project Server のバージョンは 2016 と 2019 です。"
type: docs
weight: 226
url: /ja/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

指定された Project Online アカウントまたは指定されたオンプレミスの Project Server インスタンス（Project Server のバージョン 2016 と 2019 がサポート）でプロジェクトを読み取り、操作を実行するメソッドを提供するクラスです。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | 新しい [ProjectServerManager](../../com.aspose/tasks/projectservermanager) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | デフォルトの保存オプションを使用して、Project Server\\Project Online インスタンスに新しいプロジェクトを作成します。 |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 指定された保存オプションを使用して、Project Server\\Project Online インスタンスに新しいプロジェクトを作成します。 |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Project Server の Web API にウェブリクエストが送信されたときに発生するイベントを取得します。 |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | 指定された GUID を持つプロジェクトを、Project Online アカウント \\ Project Server インスタンスから取得します。 |
| [getProjectList()](#getProjectList--) | 現在の Project Online アカウント \\ Project Server インスタンスの 'Working' ストアからプロジェクトの一覧を取得します。 |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | トラブルシューティングの目的でプロジェクトのバイナリデータを取得します。 |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Project Server の Web API にウェブリクエストが送信されたときに発生するイベントを設定します。 |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | デフォルトの保存オプションを使用して、Project Server\\Project Online インスタンスの既存プロジェクトを更新します。 |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | 指定された保存オプションを使用して、Project Server\\Project Online インスタンスの既存プロジェクトを更新します。 |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


新しい [ProjectServerManager](../../com.aspose/tasks/projectservermanager) クラスのインスタンスを初期化します。

--------------------

&gt; ```
&gt; この例では、Project Server のオンプレミスインスタンスにアクセスするための ProjectServerManager のインスタンスの作成方法を示します。
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
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Project Online アカウントに接続するために使用される認証情報です。 |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


デフォルトの保存オプションを使用して、Project Server\\Project Online インスタンスに新しいプロジェクトを作成します。

--------------------

&gt; ```
&gt; この例では、プロジェクトを .mpp ファイルからロードし、Project Online アカウントに保存します。
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
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online インスタンスに保存するプロジェクト。 |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | クラス [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) のインスタンス。 |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Project Server の Web API にウェブリクエストが送信されたときに発生するイベントを取得します。

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


指定された GUID を持つプロジェクトを、Project Online アカウント \\ Project Server インスタンスから取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| projectGuid | java.util.UUID | 読み取るプロジェクトの Guid。 |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


現在の Project Online アカウント \\ Project Server インスタンスの 'Working' ストアからプロジェクトの一覧を取得します。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - 現在の Project Online アカウント \\ Project Server インスタンス内のプロジェクトの列挙。
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


トラブルシューティングの目的でプロジェクトのバイナリデータを取得します。

--------------------

&gt; ```
&gt;
&gt; ``````

この例では、特定のプロジェクトのデバッグ情報を取得します。結果として得られた "debug.zip" をサポートチームに渡してトラブルシューティングに利用できます。
 [C#]
var credentials = new ProjectServerCredentials(\"https://xxxxxx.sharepoint.com\", \"yyyyy@xxxxxxx.onmicrosoft.com\", \"password\");
// 取得しようとしているプロジェクトの Guid。
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
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online インスタンスに保存するプロジェクト。 |

--------------------

Project のプロパティ 'project.Get(Prj.Guid)' は、Project Server アカウント \\ Project Online インスタンスに存在するプロジェクトの有効な guid である必要があります。 |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


指定された保存オプションを使用して、Project Server\\Project Online インスタンスの既存プロジェクトを更新します。既存のプロジェクトは上書きされます。

--------------------

&gt; ```
&gt; この例では、Project Online アカウントからプロジェクトをロードし、変更して、再び Project Online アカウントに保存します。
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

