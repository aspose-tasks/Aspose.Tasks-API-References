---
title: "ProjectInfo.IsCheckedOut"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ProjectInfo. Λαμβάνει μια τιμή που υποδεικνύει εάν το έργο είναι ελεγμένο"
type: docs
weight: 50
url: /el/net/aspose.tasks/projectinfo/ischeckedout/
---
## ProjectInfo.IsCheckedOut property

Λαμβάνει μια τιμή που υποδεικνύει εάν το έργο είναι ελεγχόμενο.

```csharp
public bool IsCheckedOut { get; }
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


