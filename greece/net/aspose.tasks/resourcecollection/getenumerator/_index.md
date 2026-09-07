---
title: "ResourceCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceCollection. Επιστρέφει έναν enumerator για αυτή τη συλλογή"
type: docs
weight: 80
url: /el/net/aspose.tasks/resourcecollection/getenumerator/
---
## ResourceCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<Resource> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


