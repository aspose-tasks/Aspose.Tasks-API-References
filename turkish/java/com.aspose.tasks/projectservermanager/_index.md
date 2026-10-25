---
title: "ProjectServerManager"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen Project Online hesabındaki veya belirtilen yerel Project Server örneğindeki projeleri okuma ve işlemler gerçekleştirme yöntemlerini sağlayan sınıf. Project Server sürümleri 2016 ve 2019 desteklenmektedir."
type: docs
weight: 226
url: /tr/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

Belirtilen Project Online hesabındaki veya belirtilen yerel Project Server örneğindeki projeleri okumak ve işlemler gerçekleştirmek için yöntemler sağlayan sınıf (Project Server'ın 2016 ve 2019 sürümleri desteklenir).
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Yeni bir [ProjectServerManager](../../com.aspose.tasks/projectservermanager) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Varsayılan kaydetme seçeneklerini kullanarak Project Server\Project Online örneğinde yeni bir proje oluşturur. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Belirtilen kaydetme seçeneklerini kullanarak Project Server\Project Online örneğinde yeni bir proje oluşturur. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olayı alır. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Belirtilen guid'e sahip projeyi Project Online hesabından \ Project Server örneğinden alır. |
| [getProjectList()](#getProjectList--) | Mevcut Project Online hesabının \ Project Server örneğinin 'Working' deposundan proje listesini alır. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Sorun giderme amaçları için projenin ikili verilerini alır. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olayı ayarlar. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Varsayılan kaydetme seçeneklerini kullanarak Project Server\Project Online örneğindeki mevcut projeyi günceller. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Belirtilen kaydetme seçeneklerini kullanarak Project Server\Project Online örneğindeki mevcut projeyi günceller. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Yeni bir [ProjectServerManager](../../com.aspose.tasks/projectservermanager) sınıfı örneği başlatır.

--------------------

&gt; ```
&gt; Bu örnek, Project Server'ın yerel örneğine erişmek için ProjectServerManager örneği oluşturmanın nasıl yapılacağını gösterir.
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Project Online hesabına bağlanmak için kullanılan kimlik bilgileri. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Varsayılan kaydetme seçeneklerini kullanarak Project Server\Project Online örneğinde yeni bir proje oluşturur.

--------------------

&gt; ```
&gt; Bu örnekte proje .mpp dosyasından yüklenir ve Project Online hesabına kaydedilir.
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online örneğine kaydedilecek proje. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions) sınıfının bir örneği. |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Web isteği Project Server'ın web API'sine gönderildiğinde tetiklenen bir olayı alır.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Belirtilen guid'e sahip projeyi Project Online hesabından \ Project Server örneğinden alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectGuid | java.util.UUID | Okunacak projenin Guid'i. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Mevcut Project Online hesabının \ Project Server örneğinin 'Working' deposundan proje listesini alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Mevcut Project Online hesabındaki \\ Project Server örneğindeki projelerin bir enumerasyonu.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Sorun giderme amaçları için projenin ikili verilerini alır.

--------------------

&gt; ```
&gt;
&gt; ``````

Bu örnekte belirli proje için hata ayıklama bilgileri alınır. Oluşan "debug.zip" dosyasını sorun giderme amacıyla destek ekibine gönderebilirsiniz.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Almak istediğiniz projenin Guid'i.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\\debug.zip"))
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online örneğine kaydedilecek proje. |

--------------------

Project'in 'project.Get(Prj.Guid)' özelliği, Project Server hesabı \\ Project Online örneğinde mevcut olan bir projenin geçerli guid'i olmalıdır. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Belirtilen kaydetme seçenekleri kullanılarak Project Server\\Project Online örneğindeki mevcut proje güncellenir. Mevcut proje üzerine yazılacaktır.

--------------------

&gt; ```
&gt; Bu örnekte proje Project Online hesabından yüklenir, değiştirilir ve tekrar Project Online hesabına kaydedilir.
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

