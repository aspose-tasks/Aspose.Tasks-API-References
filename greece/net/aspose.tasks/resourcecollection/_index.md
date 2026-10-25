---
title: "Κλάση ResourceCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ResourceCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων Resource"
type: docs
weight: 1770
url: /el/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στη ResourceCollection. Μόνο για ανάγνωση Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Λαμβάνει το γονικό έργο του αντικειμένου ResourceCollection. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Προσθέτει νέο πόρο στην τελευταία θέση της συλλογής πόρων ενός έργου. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Προσθέτει νέο πόρο στη συγκεκριμένη θέση της συλλογής πόρων ενός έργου. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Η άμεση εκκαθάριση δεν υποστηρίζεται, αυτή η μέθοδος απλώς ρίχνει NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Επιστρέφει έναν πόρο με το συγκεκριμένο id. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Επιστρέφει έναν πόρο με το συγκεκριμένο Uid. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Αυτή είναι η υλοποίηση stub της μεθόδου Remove του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Μετατρέπει το αντικείμενο ResourceCollection σε λίστα αντικειμένων [`Resource`](../resource/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές πόρων.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// προσθήκη κενής πόρου
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// προσθήκη πόρου με όνομα
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// προσθήκη πόρου πριν από τον πόρο με το συγκεκριμένο ID
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// λήψη πόρου με id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// Οι συλλογές πόρων δεν υποστηρίζουν την ενέργεια Clear
// project.Resources.Clear();
// χρησιμοποιήστε το επόμενο δείγμα κώδικα αντί αυτού
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Δείτε επίσης

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


