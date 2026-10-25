---
title: "ProjectServerManager.GetProjectList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ProjectServerManager. Λαμβάνει τη λίστα των έργων από το Working store του τρέχοντος λογαριασμού Project Online Project Server."
type: docs
weight: 50
url: /el/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Αποκτά τη λίστα των έργων από το αποθετήριο 'Working' του τρέχοντος λογαριασμού Project Online \ Project Server παρουσία.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Τιμή Επιστροφής

Μια απαρίθμηση των έργων στον τρέχοντα λογαριασμό Project Online \ Project Server.

## Παραδείγματα

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


