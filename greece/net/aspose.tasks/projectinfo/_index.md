---
title: "Κλάση ProjectInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectInfo. Σύντομες πληροφορίες για το δημοσιευμένο έργο που είναι διαθέσιμο στο Project Online"
type: docs
weight: 1470
url: /el/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

Σύντομες πληροφορίες για το δημοσιευμένο έργο διαθέσιμο στο Project Online.

```csharp
public sealed class ProjectInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectInfo](projectinfo/)() | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `ProjectInfo`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | Λαμβάνει την ημερομηνία και ώρα δημιουργίας του έργου. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | Λαμβάνει την περιγραφή του έργου. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | Λαμβάνει το μοναδικό αναγνωριστικό του έργου. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το έργο είναι ελεγχόμενο. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | Λαμβάνει την πιο πρόσφατη ημερομηνία δημοσίευσης του έργου. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | Λαμβάνει την πιο πρόσφατη ημερομηνία αποθήκευσης του έργου. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | Λαμβάνει το όνομα του έργου. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


