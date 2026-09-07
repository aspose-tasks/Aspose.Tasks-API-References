---
title: "ProjectInfo.ProjectInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ProjectInfo. Αρχικοποιεί μια νέα παρουσία της κλάσης ProjectInfo"
type: docs
weight: 10
url: /el/net/aspose.tasks/projectinfo/projectinfo/
---
## ProjectInfo constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`ProjectInfo`](../).

```csharp
public ProjectInfo()
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε πληροφορίες σχετικά με έργα από το Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// διαβάστε τις πληροφορίες του έργου
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### Δείτε επίσης

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


