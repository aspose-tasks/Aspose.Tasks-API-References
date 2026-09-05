---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API Reference"
description: "La classe che fornisce i metodi per leggere ed eseguire operazioni sui progetti nell'account Project Online specificato o nell'istanza di Project Server on-premise specificata. Sono supportate le versioni di Project Server 2016 e 2019."
type: docs
weight: 226
url: /it/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

La classe che fornisce i metodi per leggere e eseguire operazioni sui progetti nell'account Project Online specificato o nell'istanza on-premise di Project Server specificata (sono supportate le versioni 2016 e 2019 di Project Server).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Inizializza una nuova istanza della classe [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Crea un nuovo progetto nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio predefinite. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Crea un nuovo progetto nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio specificate. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Ottiene un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Ottiene il progetto con il GUID specificato dall'account Project Online\\ Project Server istanza. |
| [getProjectList()](#getProjectList--) | Ottiene l'elenco dei progetti dal deposito 'Working' dell'attuale account Project Online\\ Project Server istanza. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Ottiene i dati binari del progetto per scopi di troubleshooting. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Imposta un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Aggiorna un progetto esistente nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio predefinite. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Aggiorna un progetto esistente nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio specificate. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Inizializza una nuova istanza della classe [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Questo esempio mostra come creare un'istanza di ProjectServerManager per accedere all'istanza on-premise di Project Server.
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Credenziali utilizzate per connettersi all'account di Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Crea un nuovo progetto nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio predefinite.

--------------------

&gt; ```
&gt; In questo esempio il progetto viene caricato dal file .mpp e salvato nell'account di Project Online.
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Il progetto da salvare all'istanza di Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Istanza della classe [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Ottiene un evento che viene sollevato quando la richiesta web viene inviata all'API web di Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Ottiene il progetto con il GUID specificato dall'account Project Online\\ Project Server istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| projectGuid | java.util.UUID | Il Guid del progetto da leggere. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Ottiene l'elenco dei progetti dal deposito 'Working' dell'attuale account Project Online\\ Project Server istanza.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Un'enumerazione dei progetti nell'account corrente di Project Online \\ istanza di Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Ottiene i dati binari del progetto per scopi di troubleshooting.

--------------------

&gt; ```
&gt;
&gt; ``````

In questo esempio le informazioni di debug per il progetto specifico vengono recuperate. È possibile inviare il file "debug.zip" risultante al team di supporto per scopi di risoluzione dei problemi.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid del progetto che si sta tentando di ottenere.
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Il progetto da salvare all'istanza di Project Server\\Project Online. |

--------------------

La proprietà del progetto 'project.Get(Prj.Guid)' dovrebbe essere un guid valido di un progetto che esiste nell'account di Project Server \\ istanza di Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Aggiorna il progetto esistente nell'istanza di Project Server\\Project Online utilizzando le opzioni di salvataggio specificate. Il progetto esistente verrà sovrascritto.

--------------------

&gt; ```
&gt; In questo esempio il progetto viene caricato dall'account di Project Online, modificato e salvato nuovamente nell'account di Project Online.
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

