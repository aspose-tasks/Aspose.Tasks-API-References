---
title: "ProjectServerManager"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "La classe qui fournit les méthodes pour lire et effectuer des opérations sur les projets dans le compte Project Online spécifié ou dans l'instance Project Server sur site spécifiée. Les versions 2016 et 2019 de Project Server sont prises en charge."
type: docs
weight: 226
url: /fr/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

La classe qui fournit les méthodes pour lire et effectuer des opérations sur les projets dans le compte Project Online spécifié ou dans l'instance sur site de Project Server spécifiée (les versions 2016 et 2019 de Project Server sont prises en charge).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Initialise une nouvelle instance de la classe [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Crée un nouveau projet dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement par défaut. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Crée un nouveau projet dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement spécifiées. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Obtient un événement qui est déclenché lorsque la requête web est envoyée à l'API web de Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Obtient le projet avec le guid spécifié depuis le compte Project Online \\ instance Project Server. |
| [getProjectList()](#getProjectList--) | Obtient la liste des projets du magasin 'Working' du compte Project Online actuel \\ instance Project Server. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Obtient les données binaires du projet à des fins de dépannage. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Définit un événement qui est déclenché lorsque la requête web est envoyée à l'API web de Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Met à jour le projet existant dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement par défaut. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Met à jour le projet existant dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement spécifiées. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Initialise une nouvelle instance de la classe [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Cet exemple montre comment créer une instance de ProjectServerManager pour accéder à l'instance sur site de Project Server.
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
| Paramètre | Type | Description |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Identifiants utilisés pour se connecter au compte Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Crée un nouveau projet dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement par défaut.

--------------------

&gt; ```
&gt; Dans cet exemple, le projet est chargé à partir d'un fichier .mpp et enregistré dans le compte Project Online.
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
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Le projet à enregistrer dans l'instance Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instance de la classe [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Obtient un événement qui est déclenché lorsque la requête web est envoyée à l'API web de Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Obtient le projet avec le guid spécifié depuis le compte Project Online \\ instance Project Server.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| projectGuid | java.util.UUID | Le Guid du projet à lire. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Obtient la liste des projets du magasin 'Working' du compte Project Online actuel \\ instance Project Server.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Une énumération des projets dans le compte Project Online actuel \\ instance Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Obtient les données binaires du projet à des fins de dépannage.

--------------------

&gt; ```
&gt;
&gt; ``````

Dans cet exemple, les informations de débogage du projet spécifique sont récupérées. Vous pouvez transmettre le fichier "debug.zip" résultant à l'équipe de support à des fins de dépannage.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid du projet que vous essayez d'obtenir.
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
| Paramètre | Type | Description |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Le projet à enregistrer dans l'instance Project Server\\Project Online. |

--------------------

La propriété du projet 'project.Get(Prj.Guid)' doit être un guid valide d'un projet qui existe dans le compte Project Server \\ instance Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Met à jour le projet existant dans l'instance Project Server\\Project Online en utilisant les options d'enregistrement spécifiées. Le projet existant sera écrasé.

--------------------

&gt; ```
&gt; Dans cet exemple, le projet est chargé depuis le compte Project Online, modifié et enregistré à nouveau dans le compte Project Online.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("Nouvelle tâche");
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

