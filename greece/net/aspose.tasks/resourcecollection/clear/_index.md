---
title: "ResourceCollection.Clear"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceCollection. Η άμεση εκκαθάριση δεν υποστηρίζεται, αυτή η μέθοδος απλώς ρίχνει NotSupportedException"
type: docs
weight: 50
url: /el/net/aspose.tasks/resourcecollection/clear/
---
## ResourceCollection.Clear method

Η άμεση εκκαθάριση δεν υποστηρίζεται, αυτή η μέθοδος απλώς ρίχνει NotSupportedException.

```csharp
public void Clear()
```

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

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


