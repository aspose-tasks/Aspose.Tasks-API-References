---
title: "ProjectServerManager"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "La clase que proporciona los métodos para leer y realizar operaciones en proyectos en la cuenta de Project Online especificada o en la instancia de Project Server local especificada. Se admiten versiones de Project Server 2016 y 2019."
type: docs
weight: 226
url: /es/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

La clase que proporciona los métodos para leer y realizar operaciones en proyectos en la cuenta especificada de Project Online o en la instancia especificada local de Project Server (se admiten las versiones 2016 y 2019 de Project Server).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Inicializa una nueva instancia de la clase [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Métodos

| Método | Descripción |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Crea un nuevo proyecto en la instancia de Project Server\\Project Online usando las opciones de guardado predeterminadas. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Crea un nuevo proyecto en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Obtiene un evento que se dispara cuando la solicitud web se envía a la API web de Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Obtiene el proyecto con el GUID especificado de la cuenta de Project Online \\ instancia de Project Server. |
| [getProjectList()](#getProjectList--) | Obtiene la lista de proyectos del almacén 'Working' de la cuenta actual de Project Online \\ instancia de Project Server. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Obtiene los datos binarios del proyecto con fines de solución de problemas. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Establece un evento que se dispara cuando la solicitud web se envía a la API web de Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Actualiza un proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado predeterminadas. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Actualiza un proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Inicializa una nueva instancia de la clase [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Este ejemplo muestra cómo crear una instancia de ProjectServerManager para acceder a la instancia local de Project Server.
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Credenciales usadas para conectar a la cuenta de Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Crea un nuevo proyecto en la instancia de Project Server\\Project Online usando las opciones de guardado predeterminadas.

--------------------

&gt; ```
&gt; En este ejemplo el proyecto se carga desde un archivo .mpp y se guarda en la cuenta de Project Online.
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | El proyecto a guardar en la instancia de Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instancia de la clase [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Obtiene un evento que se dispara cuando la solicitud web se envía a la API web de Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Obtiene el proyecto con el GUID especificado de la cuenta de Project Online \\ instancia de Project Server.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectGuid | java.util.UUID | El Guid del proyecto a leer. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Obtiene la lista de proyectos del almacén 'Working' de la cuenta actual de Project Online \\ instancia de Project Server.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Una enumeración de proyectos en la cuenta actual de Project Online \\ instancia de Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Obtiene los datos binarios del proyecto con fines de solución de problemas.

--------------------

&gt; ```
&gt;
&gt; ``````

En este ejemplo se recupera la información de depuración del proyecto específico. Puedes pasar el archivo resultante "debug.zip" al equipo de soporte para fines de solución de problemas.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid del proyecto que estás intentando obtener.
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | El proyecto a guardar en la instancia de Project Server\\Project Online. |

--------------------

La propiedad del proyecto 'project.Get(Prj.Guid)' debe ser un guid válido de un proyecto que exista en la cuenta de Project Server \\ instancia de Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Actualiza el proyecto existente en la instancia de Project Server\\Project Online usando las opciones de guardado especificadas. El proyecto existente será sobrescrito.

--------------------

&gt; ```
&gt; En este ejemplo el proyecto se carga desde la cuenta de Project Online, se modifica y se guarda de nuevo en la cuenta de Project Online.
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

