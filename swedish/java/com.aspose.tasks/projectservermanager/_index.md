---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API-referens"
description: "Klassen som tillhandahåller metoder för att läsa och utföra operationer på projekt i det angivna Project Online‑kontot eller i den angivna lokala Project Server‑instansen. Versioner av Project Server 2016 och 2019 stöds."
type: docs
weight: 226
url: /sv/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

Klassen som tillhandahåller metoderna för att läsa och utföra operationer på projekt i det angivna Project Online-kontot eller i den angivna lokala Project Server-instansen (versionerna 2016 och 2019 av Project Server stöds).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Initierar en ny instans av klassen [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Skapar ett nytt projekt i Project Server\Project Online‑instans med standard sparalternativ. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Skapar ett nytt projekt i Project Server\Project Online‑instans med de angivna sparalternativen. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Hämtar en händelse som utlöses när webbrequesten skickas till Project Server:s webb‑API. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Hämtar projektet med det angivna guid‑värdet från Project Online‑kontot \ Project Server‑instansen. |
| [getProjectList()](#getProjectList--) | Hämtar listan över projekt från 'Working'-lagret i det aktuella Project Online‑kontot \\ Project Server‑instansen. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Hämtar projektets binära data för felsökningsändamål. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Ställer in en händelse som utlöses när webbförfrågan skickas till Project Servers webb‑API. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Uppdaterar befintligt projekt i Project Server\\Project Online‑instansen med standardalternativ för sparande. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Uppdaterar befintligt projekt i Project Server\\Project Online‑instansen med de angivna sparalternativen. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Initierar en ny instans av klassen [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Detta exempel visar hur man skapar en instans av ProjectServerManager för att komma åt en lokal instans av Project Server.
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Referenser som används för att ansluta till Project Online‑kontot. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Skapar ett nytt projekt i Project Server\Project Online‑instans med standard sparalternativ.

--------------------

&gt; ```
&gt; I detta exempel laddas projektet från en .mpp‑fil och sparas till Project Online‑kontot.
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projektet som ska sparas till Project Server\\Project Online‑instansen. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instans av klassen [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Hämtar en händelse som utlöses när webbrequesten skickas till Project Server:s webb‑API.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Hämtar projektet med det angivna guid‑värdet från Project Online‑kontot \ Project Server‑instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| projectGuid | java.util.UUID | Guid för projektet som ska läsas. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Hämtar listan över projekt från 'Working'-lagret i det aktuella Project Online‑kontot \\ Project Server‑instansen.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - En uppräkning av projekt i det aktuella Project Online‑kontot \\ Project Server‑instansen.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Hämtar projektets binära data för felsökningsändamål.

--------------------

&gt; ```
&gt;
&gt; ``````

I detta exempel hämtas felsökningsinformationen för det specifika projektet. Du kan skicka den resulterande "debug.zip" till supportteamet för felsökning.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid för projektet du försöker hämta.
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Projektet som ska sparas till Project Server\\Project Online‑instansen. |

--------------------

Projektets egenskap 'project.Get(Prj.Guid)' ska vara en giltig guid för ett projekt som finns i Project Server‑konto \\ Project Online‑instans. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Uppdaterar befintligt projekt i Project Server\\Project Online‑instans med de angivna sparalternativen. Det befintliga projektet kommer att skrivas över.

--------------------

&gt; ```
&gt; I det här exemplet laddas projektet från Project Online‑konto, modifieras och sparas tillbaka till Project Online‑konto.
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

