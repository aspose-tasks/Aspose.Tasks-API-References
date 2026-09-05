---
title: "ProjectServerManager"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "वह क्लास जो निर्दिष्ट Project Online खाते या निर्दिष्ट ऑन‑प्रिमाइसेस Project Server इंस्टेंस में प्रोजेक्ट्स को पढ़ने और संचालन करने के लिए विधियाँ प्रदान करती है, Project Server के संस्करण 2016 और 2019 समर्थित हैं।"
type: docs
weight: 226
url: /hi/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

वह क्लास जो निर्दिष्ट Project Online अकाउंट या निर्दिष्ट ऑन-प्रेमाइस Project Server इंस्टेंस में प्रोजेक्ट्स को पढ़ने और ऑपरेशन्स करने के लिए मेथड्स प्रदान करती है (Project Server के संस्करण 2016 और 2019 समर्थित हैं)।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | नए [ProjectServerManager](../../com.aspose.tasks/projectservermanager) क्लास का एक नया इंस्टेंस प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है। |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है। |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | जब वेब अनुरोध Project Server की वेब API को भेजा जाता है, तब उत्पन्न होने वाली इवेंट प्राप्त करता है। |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | निर्दिष्ट GUID वाले प्रोजेक्ट को Project Online खाते \\ Project Server इंस्टेंस से प्राप्त करता है। |
| [getProjectList()](#getProjectList--) | वर्तमान Project Online खाते \\ Project Server इंस्टेंस के 'Working' स्टोर से प्रोजेक्ट्स की सूची प्राप्त करता है। |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | समस्या निवारण के उद्देश्य से प्रोजेक्ट का बाइनरी डेटा प्राप्त करता है। |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | जब वेब अनुरोध Project Server की वेब API को भेजा जाता है, तब उत्पन्न होने वाली इवेंट सेट करता है। |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


नए [ProjectServerManager](../../com.aspose.tasks/projectservermanager) क्लास का एक नया इंस्टेंस प्रारंभ करता है।

--------------------

&gt; ```
&gt; यह उदाहरण दिखाता है कि ProjectServerManager का इंस्टेंस कैसे बनाकर Project Server के ऑन‑प्रिमाइसेस इंस्टेंस तक पहुंचा जाए।
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Project Online खाते से कनेक्ट करने के लिए उपयोग किए जाने वाले क्रेडेंशियल्स। |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


डिफ़ॉल्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में नया प्रोजेक्ट बनाता है।

--------------------

&gt; ```
&gt; इस उदाहरण में प्रोजेक्ट .mpp फ़ाइल से लोड किया जाता है और Project Online खाते में सहेजा जाता है।
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) क्लास का उदाहरण। |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


जब वेब अनुरोध Project Server की वेब API को भेजा जाता है, तब उत्पन्न होने वाली इवेंट प्राप्त करता है।

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


निर्दिष्ट GUID वाले प्रोजेक्ट को Project Online खाते \\ Project Server इंस्टेंस से प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| projectGuid | java.util.UUID | पढ़ने के लिए प्रोजेक्ट का Guid। |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


वर्तमान Project Online खाते \\ Project Server इंस्टेंस के 'Working' स्टोर से प्रोजेक्ट्स की सूची प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - वर्तमान Project Online खाते \\ Project Server इंस्टेंस में प्रोजेक्ट्स की एक सूची।
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


समस्या निवारण के उद्देश्य से प्रोजेक्ट का बाइनरी डेटा प्राप्त करता है।

--------------------

&gt; ```
&gt;
&gt; ``````

इस उदाहरण में विशिष्ट प्रोजेक्ट के लिए डिबग जानकारी प्राप्त की जाती है। आप प्राप्त "debug.zip" को समस्या निवारण के लिए सपोर्ट टीम को पास कर सकते हैं।
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// आप जिस प्रोजेक्ट का Guid प्राप्त करना चाहते हैं।
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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Project Server\\Project Online इंस्टेंस में सहेजने के लिए प्रोजेक्ट। |

--------------------

Project का प्रॉपर्टी 'project.Get(Prj.Guid)' एक वैध guid होना चाहिए जो Project Server खाते \\ Project Online इंस्टेंस में मौजूद प्रोजेक्ट का हो। |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


निर्दिष्ट सहेजने विकल्पों का उपयोग करके Project Server\\Project Online इंस्टेंस में मौजूदा प्रोजेक्ट को अपडेट करता है। मौजूदा प्रोजेक्ट को ओवरराइट कर दिया जाएगा।

--------------------

&gt; ```
&gt; इस उदाहरण में प्रोजेक्ट को Project Online खाते से लोड किया जाता है, संशोधित किया जाता है और फिर Project Online खाते में वापस सहेजा जाता है।
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

