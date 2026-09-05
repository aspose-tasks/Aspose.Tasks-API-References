---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API-referentie"
description: "De klasse die de methoden biedt om projecten te lezen en bewerkingen uit te voeren in het opgegeven Project Online‑account of in de opgegeven on‑premise Project Server‑instantie. Project Server‑versies 2016 en 2019 worden ondersteund."
type: docs
weight: 226
url: /nl/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

De klasse die de methoden biedt om projecten te lezen en bewerkingen uit te voeren in het opgegeven Project Online‑account of in de opgegeven on‑premise‑Project Server‑instantie (versies 2016 en 2019 van Project Server worden ondersteund).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Initialiseert een nieuw exemplaar van de [ProjectServerManager](../../com.aspose.tasks/projectservermanager) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Maakt een nieuw project aan in de Project Server\\Project Online‑instantie met behulp van de standaard opslagopties. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Maakt een nieuw project aan in de Project Server\\Project Online‑instantie met behulp van de opgegeven opslagopties. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Haalt een gebeurtenis op die wordt opgewekt wanneer het webverzoek wordt verzonden naar de web‑API van Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Haalt het project op met de opgegeven guid uit het Project Online‑account \\ Project Server‑instantie. |
| [getProjectList()](#getProjectList--) | Haalt de lijst met projecten op uit de 'Working'-opslag van het huidige Project Online‑account \\ Project Server‑instantie. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Haalt de binaire gegevens van het project op voor probleemoplossingsdoeleinden. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Stelt een gebeurtenis in die wordt opgewekt wanneer het webverzoek wordt verzonden naar de web‑API van Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Werkt een bestaand project bij in de Project Server\\Project Online‑instantie met behulp van de standaard opslagopties. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Werkt een bestaand project bij in de Project Server\\Project Online‑instantie met behulp van de opgegeven opslagopties. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Initialiseert een nieuw exemplaar van de [ProjectServerManager](../../com.aspose.tasks/projectservermanager) klasse.

--------------------

&gt; ```
&gt; Dit voorbeeld laat zien hoe een instantie van ProjectServerManager te maken om toegang te krijgen tot een on‑premise instantie van Project Server.
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Referenties die worden gebruikt om verbinding te maken met een Project Online-account. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Maakt een nieuw project aan in de Project Server\\Project Online‑instantie met behulp van de standaard opslagopties.

--------------------

&gt; ```
&gt; In dit voorbeeld wordt het project geladen vanuit een .mpp-bestand en opgeslagen in een Project Online-account.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxx.onmicrosoft.com", "password");
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Het project om op te slaan naar de Project Server\\Project Online-instantie. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instantie van de klasse [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Haalt een gebeurtenis op die wordt opgewekt wanneer het webverzoek wordt verzonden naar de web‑API van Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Haalt het project op met de opgegeven guid uit het Project Online‑account \\ Project Server‑instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| projectGuid | java.util.UUID | De Guid van het project om te lezen. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Haalt de lijst met projecten op uit de 'Working'-opslag van het huidige Project Online‑account \\ Project Server‑instantie.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Een opsomming van projecten in het huidige Project Online-account \\ Project Server-instantie.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Haalt de binaire gegevens van het project op voor probleemoplossingsdoeleinden.

--------------------

&gt; ```
&gt;
&gt; ``````

In dit voorbeeld wordt de debug‑informatie voor het specifieke project opgehaald. Je kunt het resulterende "debug.zip" doorsturen naar het ondersteuningsteam voor probleemoplossingsdoeleinden.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxx.onmicrosoft.com", "password");
// Guid van het project dat je probeert op te halen.
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Het project om op te slaan naar de Project Server\\Project Online-instantie. |

--------------------

De eigenschap van het project 'project.Get(Prj.Guid)' moet een geldige guid zijn van een project dat bestaat in de Project Server-account \\ Project Online-instantie. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Werkt een bestaand project bij in de Project Server\\Project Online-instantie met behulp van de opgegeven opslagopties. Het bestaande project wordt overschreven.

--------------------

&gt; ```
&gt; In dit voorbeeld wordt het project geladen vanuit een Project Online-account, aangepast en terug opgeslagen naar het Project Online-account.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxx.onmicrosoft.com", "password");
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

