---
title: "ProjectServerManager.GetProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ProjectServerManager μέθοδος. Αποκτά το έργο με το καθορισμένο guid από τον λογαριασμό Project Online του παραδείγματος Project Server"
type: docs
weight: 40
url: /el/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Αποκτά το έργο με το καθορισμένο guid από τον λογαριασμό Project Online \ Project Server παρουσία.

```csharp
public Project GetProject(Guid projectGuid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| projectGuid | Guid | Το Guid του έργου που θα διαβαστεί. |

### Τιμή Επιστροφής

Παράδειγμα της κλάσης [`Project`](../../project/) που αντιπροσωπεύει το έργο που διαβάστηκε από το Project Online \\ Project Server.

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


