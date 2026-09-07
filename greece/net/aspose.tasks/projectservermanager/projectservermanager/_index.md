---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ProjectServerManager. Αρχικοποιεί μια νέα παρουσία της κλάσης ProjectServerManager."
type: docs
weight: 10
url: /el/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαπιστευτήρια | ProjectServerCredentials | Διαπιστευτήρια που χρησιμοποιούνται για σύνδεση με λογαριασμό Project Online. |

## Παραδείγματα

Αυτό το παράδειγμα δείχνει πώς να δημιουργήσετε μια παρουσία του ProjectServerManager για πρόσβαση σε τοπική παρουσία του Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Αυτό το παράδειγμα δείχνει πώς να δημιουργήσετε μια παρουσία του ProjectServerManager για πρόσβαση σε λογαριασμό στην υπηρεσία Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Δείχνει πώς να διαβάσετε ένα έργο από το Microsoft Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### Δείτε επίσης

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


