---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API Reference"
description: "Die Klasse, die Methoden zum Lesen und Ausführen von Vorgängen an Projekten im angegebenen Project Online-Konto oder in der angegebenen lokalen Project Server-Instanz bereitstellt. Project Server-Versionen 2016 und 2019 werden unterstützt."
type: docs
weight: 226
url: /de/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

Die Klasse, die die Methoden zum Lesen und Ausführen von Operationen an Projekten im angegebenen Project Online-Konto oder in der angegebenen lokalen Project Server-Instanz bereitstellt (Versionen 2016 und 2019 von Project Server werden unterstützt).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Initialisiert eine neue Instanz der Klasse [ProjectServerManager](../../com.aspose/tasks/projectservermanager). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Erstellt ein neues Projekt in einer Project Server\\Project Online-Instanz mit den standardmäßigen Speicheroptionen. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Erstellt ein neues Projekt in einer Project Server\\Project Online-Instanz mit den angegebenen Speicheroptionen. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Ruft ein Ereignis ab, das ausgelöst wird, wenn die Webanfrage an die Web‑API von Project Server gesendet wird. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Ruft das Projekt mit der angegebenen GUID aus dem Project Online‑Konto \\ Project Server‑Instanz ab. |
| [getProjectList()](#getProjectList--) | Ruft die Liste der Projekte aus dem 'Working'-Speicher des aktuellen Project Online‑Kontos \\ Project Server‑Instanz ab. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Ruft die Binärdaten des Projekts zu Fehlersuchzwecken ab. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn die Webanfrage an die Web‑API von Project Server gesendet wird. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Aktualisiert ein vorhandenes Projekt in einer Project Server\\Project Online‑Instanz mit den standardmäßigen Speicheroptionen. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Aktualisiert ein vorhandenes Projekt in einer Project Server\\Project Online‑Instanz mit den angegebenen Speicheroptionen. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Initialisiert eine neue Instanz der Klasse [ProjectServerManager](../../com.aspose/tasks/projectservermanager).

--------------------

&gt; ```
&gt; Dieses Beispiel zeigt, wie man eine Instanz von ProjectServerManager erstellt, um auf eine lokale Instanz von Project Server zuzugreifen.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Anmeldeinformationen, die verwendet werden, um eine Verbindung zum Project Online‑Konto herzustellen. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Erstellt ein neues Projekt in einer Project Server\\Project Online-Instanz mit den standardmäßigen Speicheroptionen.

--------------------

&gt; ```
&gt; In diesem Beispiel wird das Projekt aus einer .mpp-Datei geladen und im Project Online-Konto gespeichert.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Das Projekt, das in die Project Server\\Project Online-Instanz gespeichert werden soll. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instanz der Klasse [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Ruft ein Ereignis ab, das ausgelöst wird, wenn die Webanfrage an die Web‑API von Project Server gesendet wird.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Ruft das Projekt mit der angegebenen GUID aus dem Project Online‑Konto \\ Project Server‑Instanz ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| projectGuid | java.util.UUID | Die Guid des zu lesenden Projekts. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Ruft die Liste der Projekte aus dem 'Working'-Speicher des aktuellen Project Online‑Kontos \\ Project Server‑Instanz ab.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Eine Aufzählung von Projekten im aktuellen Project Online‑Konto \\ Project Server‑Instanz.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Ruft die Binärdaten des Projekts zu Fehlersuchzwecken ab.

--------------------

&gt; ```
&gt;
&gt; ``````

In diesem Beispiel werden die Debug‑Informationen für das jeweilige Projekt abgerufen. Sie können die resultierende "debug.zip" an das Support‑Team zu Fehlersuchzwecken weitergeben.
 [C#]
var credentials = new ProjectServerCredentials(\"https://xxxxxx.sharepoint.com\", \"yyyyy@xxxxxxx.onmicrosoft.com\", \"password\");
// Guid des Projekts, das Sie abrufen möchten.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Das Projekt, das in die Project Server\\Project Online-Instanz gespeichert werden soll. |

--------------------

Die Eigenschaft 'project.Get(Prj.Guid)' des Projekts sollte eine gültige Guid eines Projekts sein, das im Project Server‑Konto \\ Project Online‑Instanz existiert. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Aktualisiert ein vorhandenes Projekt in der Project Server\\Project Online‑Instanz mit den angegebenen Speicheroptionen. Das vorhandene Projekt wird überschrieben.

--------------------

&gt; ```
&gt; In diesem Beispiel wird das Projekt aus dem Project Online‑Konto geladen, geändert und zurück in das Project Online‑Konto gespeichert.
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

