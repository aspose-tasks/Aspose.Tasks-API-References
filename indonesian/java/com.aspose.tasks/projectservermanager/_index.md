---
title: "ProjectServerManager"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas yang menyediakan metode untuk membaca dan melakukan operasi pada proyek dalam akun Project Online yang ditentukan atau dalam instance Project Server on‑premise yang ditentukan. Versi Project Server 2016 dan 2019 didukung."
type: docs
weight: 226
url: /id/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

Kelas yang menyediakan metode untuk membaca dan melakukan operasi pada proyek dalam akun Project Online yang ditentukan atau dalam instance Project Server on-premise yang ditentukan (versi Project Server 2016 dan 2019 didukung).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Menginisialisasi instance baru dari kelas [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Membuat proyek baru dalam instance Project Server\\Project Online menggunakan opsi penyimpanan default. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Membuat proyek baru dalam instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Mendapatkan peristiwa yang dipicu ketika permintaan web dikirim ke API web Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Mendapatkan proyek dengan guid yang ditentukan dari akun Project Online \\ instance Project Server. |
| [getProjectList()](#getProjectList--) | Mendapatkan daftar proyek dari penyimpanan 'Working' akun Project Online \\ instance Project Server saat ini. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Mendapatkan data biner proyek untuk keperluan pemecahan masalah. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Menetapkan peristiwa yang dipicu ketika permintaan web dikirim ke API web Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Memperbarui proyek yang ada dalam instance Project Server\\Project Online menggunakan opsi penyimpanan default. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Memperbarui proyek yang ada dalam instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Menginisialisasi instance baru dari kelas [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Contoh ini menunjukkan cara membuat instance ProjectServerManager untuk mengakses instance on-premise Project Server.
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Kredensial yang digunakan untuk terhubung ke akun Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Membuat proyek baru dalam instance Project Server\\Project Online menggunakan opsi penyimpanan default.

--------------------

&gt; ```
&gt; Dalam contoh ini proyek dimuat dari file .mpp dan disimpan ke akun Project Online.
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyek yang akan disimpan ke instance Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Instansi dari kelas [ProjectServerSaveOptions](../../com.aspose/tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Mendapatkan peristiwa yang dipicu ketika permintaan web dikirim ke API web Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Mendapatkan proyek dengan guid yang ditentukan dari akun Project Online \\ instance Project Server.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectGuid | java.util.UUID | Guid proyek yang akan dibaca. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Mendapatkan daftar proyek dari penyimpanan 'Working' akun Project Online \\ instance Project Server saat ini.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Sebuah enumerasi proyek dalam akun Project Online saat ini \\ instance Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Mendapatkan data biner proyek untuk keperluan pemecahan masalah.

--------------------

&gt; ```
&gt;
&gt; ``````

Dalam contoh ini info debug untuk proyek tertentu diambil. Anda dapat mengirimkan "debug.zip" yang dihasilkan ke tim dukungan untuk tujuan pemecahan masalah.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid proyek yang ingin Anda dapatkan.
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Proyek yang akan disimpan ke instance Project Server\\Project Online. |

--------------------

Properti 'project.Get(Prj.Guid)' pada Project harus berupa guid yang valid dari proyek yang ada di akun Project Server \\ instance Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Memperbarui proyek yang ada di instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. Proyek yang ada akan ditimpa.

--------------------

&gt; ```
&gt; Dalam contoh ini proyek dimuat dari akun Project Online, dimodifikasi, dan disimpan kembali ke akun Project Online.
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

