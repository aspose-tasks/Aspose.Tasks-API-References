---
title: "ProjectServerManager"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "الفئة التي توفر الطرق لقراءة وتنفيذ العمليات على المشاريع في حساب Project Online المحدد أو في مثيل Project Server المحلي المحدد. يتم دعم إصدارات Project Server 2016 و 2019."
type: docs
weight: 226
url: /ar/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

الفئة التي توفر الأساليب لقراءة المشاريع وإجراء عمليات عليها في حساب Project Online المحدد أو في مثيل Project Server المحلي المحدد (تُدعم إصدارات Project Server 2016 و2019).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | يُهيئ مثيلًا جديدًا من الفئة [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | ينشئ مشروعًا جديدًا في مثيل Project Server\\Project Online باستخدام خيارات الحفظ الافتراضية. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | ينشئ مشروعًا جديدًا في مثيل Project Server\\Project Online باستخدام خيارات الحفظ المحددة. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | يحصل على حدث يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات الويب الخاصة بـ Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | يحصل على المشروع بالمعرف المحدد من حساب Project Online \\ مثيل Project Server. |
| [getProjectList()](#getProjectList--) | يحصل على قائمة المشاريع من مخزن 'Working' لحساب Project Online الحالي \\ مثيل Project Server. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | يضبط حدثًا يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات الويب الخاصة بـ Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | يحدّث المشروع الموجود في مثيل Project Server\\Project Online باستخدام خيارات الحفظ الافتراضية. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | يحدّث المشروع الموجود في مثيل Project Server\\Project Online باستخدام خيارات الحفظ المحددة. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


يُهيئ مثيلًا جديدًا من الفئة [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; يوضح هذا المثال كيفية إنشاء مثيل من ProjectServerManager للوصول إلى مثيل Project Server المحلي.
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | بيانات الاعتماد المستخدمة للاتصال بحساب Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


ينشئ مشروعًا جديدًا في مثيل Project Server\\Project Online باستخدام خيارات الحفظ الافتراضية.

--------------------

&gt; ```
&gt; في هذا المثال يتم تحميل المشروع من ملف .mpp وحفظه إلى حساب Project Online.
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | المشروع لحفظه إلى مثيل Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | مثال على الفئة [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


يحصل على حدث يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات الويب الخاصة بـ Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


يحصل على المشروع بالمعرف المحدد من حساب Project Online \\ مثيل Project Server.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectGuid | java.util.UUID | معرف Guid للمشروع المراد قراءته. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


يحصل على قائمة المشاريع من مخزن 'Working' لحساب Project Online الحالي \\ مثيل Project Server.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - تعداد للمشروعات في حساب Project Online الحالي \\ مثيل Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها.

--------------------

&gt; ```
&gt;
&gt; ``````

في هذا المثال يتم استرجاع معلومات التصحيح للمشروع المحدد. يمكنك تمرير الملف الناتج "debug.zip" إلى فريق الدعم لأغراض استكشاف الأخطاء وإصلاحها.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// معرف Guid للمشروع الذي تحاول الحصول عليه.
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
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | المشروع لحفظه إلى مثيل Project Server\\Project Online. |

--------------------

خاصية المشروع 'project.Get(Prj.Guid)' يجب أن تكون guid صالحة لمشروع موجود في حساب Project Server \\ مثيل Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


يقوم بتحديث المشروع الموجود في مثيل Project Server\\Project Online باستخدام خيارات الحفظ المحددة. سيتم استبدال المشروع الحالي.

--------------------

&gt; ```
&gt; في هذا المثال يتم تحميل المشروع من حساب Project Online، تعديلّه وحفظه مرة أخرى إلى حساب Project Online.
&gt; ``````

 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("مهمة جديدة");
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

