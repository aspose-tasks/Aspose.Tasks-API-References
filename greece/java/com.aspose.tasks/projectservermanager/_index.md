---
title: "ProjectServerManager"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Η κλάση που παρέχει τις μεθόδους για ανάγνωση και εκτέλεση λειτουργιών σε έργα στον καθορισμένο λογαριασμό Project Online ή στην καθορισμένη τοπική εγκατάσταση Project Server. Υποστηρίζονται εκδόσεις Project Server 2016 και 2019."
type: docs
weight: 226
url: /el/java/com.aspose.tasks/projectservermanager/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerManager
```

Η κλάση που παρέχει τις μεθόδους για ανάγνωση και εκτέλεση λειτουργιών σε έργα στον καθορισμένο λογαριασμό Project Online ή στην καθορισμένη τοπική παρουσία του Project Server (υποστηρίζονται οι εκδόσεις Project Server 2016 και 2019).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProjectServerManager(ProjectServerCredentials credentials)](#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [ProjectServerManager](../../com.aspose.tasks/projectservermanager). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [createNewProject(Project project)](#createNewProject-com.aspose.tasks.Project-) | Δημιουργεί νέο έργο στην εγκατάσταση Project Server\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. |
| [createNewProject(Project project, ProjectServerSaveOptions saveOptions)](#createNewProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Δημιουργεί νέο έργο στην εγκατάσταση Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [getExecutingWebRequest()](#getExecutingWebRequest--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν το web request αποστέλλεται στο web API του Project Server. |
| [getProject(UUID projectGuid)](#getProject-java.util.UUID-) | Λαμβάνει το έργο με το καθορισμένο guid από τον λογαριασμό Project Online \ την εγκατάσταση Project Server. |
| [getProjectList()](#getProjectList--) | Λαμβάνει τη λίστα των έργων από το κατάστημα 'Working' του τρέχοντος λογαριασμού Project Online \ της εγκατάστασης Project Server. |
| [getProjectRawData(UUID projectGuid)](#getProjectRawData-java.util.UUID-) | Λαμβάνει τα δυαδικά δεδομένα του έργου για σκοπούς αντιμετώπισης προβλημάτων. |
| [setExecutingWebRequest(Event&lt;WebRequestEventArgs&gt; value)](#setExecutingWebRequest-com.aspose.tasks.Event-com.aspose.tasks.WebRequestEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν το web request αποστέλλεται στο web API του Project Server. |
| [updateProject(Project project)](#updateProject-com.aspose.tasks.Project-) | Ενημερώνει υπάρχον έργο στην εγκατάσταση Project Server\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης. |
| [updateProject(Project project, ProjectServerSaveOptions saveOptions)](#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-) | Ενημερώνει υπάρχον έργο στην εγκατάσταση Project Server\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
### ProjectServerManager(ProjectServerCredentials credentials) {#ProjectServerManager-com.aspose.tasks.ProjectServerCredentials-}
```
public ProjectServerManager(ProjectServerCredentials credentials)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [ProjectServerManager](../../com.aspose.tasks/projectservermanager).

--------------------

&gt; ```
&gt; Αυτό το παράδειγμα δείχνει πώς να δημιουργήσετε ένα παράδειγμα του ProjectServerManager για πρόσβαση στην τοπική εγκατάσταση του Project Server.
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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| credentials | [ProjectServerCredentials](../../com.aspose.tasks/projectservercredentials) | Διαπιστευτήρια που χρησιμοποιούνται για σύνδεση στον λογαριασμό Project Online. |

### createNewProject(Project project) {#createNewProject-com.aspose.tasks.Project-}
```
public final void createNewProject(Project project)
```


Δημιουργεί νέο έργο στην εγκατάσταση Project Server\Project Online χρησιμοποιώντας τις προεπιλεγμένες επιλογές αποθήκευσης.

--------------------

&gt; ```
&gt; Σε αυτό το παράδειγμα το έργο φορτώνεται από αρχείο .mpp και αποθηκεύεται στον λογαριασμό Project Online.
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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Το έργο για αποθήκευση σε παρουσία Project Server\\Project Online. |
| saveOptions | [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions) | Παράδειγμα της κλάσης [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |

### getExecutingWebRequest() {#getExecutingWebRequest--}
```
public final Event<WebRequestEventArgs> getExecutingWebRequest()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν το web request αποστέλλεται στο web API του Project Server.

**Returns:**
[Event](../../com.aspose.tasks/event) - an event that is raised when the web request is sent to Project Server's web API.
### getProject(UUID projectGuid) {#getProject-java.util.UUID-}
```
public final Project getProject(UUID projectGuid)
```


Λαμβάνει το έργο με το καθορισμένο guid από τον λογαριασμό Project Online \ την εγκατάσταση Project Server.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectGuid | java.util.UUID | Το Guid του έργου για ανάγνωση. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Instance of [Project](../../com.aspose.tasks/project) class which represents project read from Project Online \\ Project Server.
### getProjectList() {#getProjectList--}
```
public final Iterable<ProjectInfo> getProjectList()
```


Λαμβάνει τη λίστα των έργων από το κατάστημα 'Working' του τρέχοντος λογαριασμού Project Online \ της εγκατάστασης Project Server.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.ProjectInfo&gt; - Μια απαρίθμηση των έργων στον τρέχον λογαριασμό Project Online \\ παρουσία Project Server.
### getProjectRawData(UUID projectGuid) {#getProjectRawData-java.util.UUID-}
```
public final InputStream getProjectRawData(UUID projectGuid)
```


Λαμβάνει τα δυαδικά δεδομένα του έργου για σκοπούς αντιμετώπισης προβλημάτων.

--------------------

&gt; ```
&gt;
&gt; ``````

Σε αυτό το παράδειγμα λαμβάνονται οι πληροφορίες εντοπισμού σφαλμάτων για το συγκεκριμένο έργο. Μπορείτε να στείλετε το παραγόμενο "debug.zip" στην ομάδα υποστήριξης για σκοπούς αντιμετώπισης προβλημάτων.
 [C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// Guid του έργου που προσπαθείτε να λάβετε.
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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | project | [Project](../../com.aspose.tasks/project) | Το έργο για αποθήκευση σε παρουσία Project Server\\Project Online. |

--------------------

Η ιδιότητα του Project 'project.Get(Prj.Guid)' πρέπει να είναι ένα έγκυρο guid ενός έργου που υπάρχει στον λογαριασμό Project Server \\ παρουσία Project Online. |

### updateProject(Project project, ProjectServerSaveOptions saveOptions) {#updateProject-com.aspose.tasks.Project-com.aspose.tasks.ProjectServerSaveOptions-}
```
public final void updateProject(Project project, ProjectServerSaveOptions saveOptions)
```


Ενημερώνει υπάρχον έργο στην παρουσία Project Server\\Project Online χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. Το υπάρχον έργο θα αντικατασταθεί.

--------------------

&gt; ```
&gt; Σε αυτό το παράδειγμα το έργο φορτώνεται από λογαριασμό Project Online, τροποποιείται και αποθηκεύεται ξανά στον λογαριασμό Project Online.
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

