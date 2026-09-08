---
title: "Klasse ResourceCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ResourceCollection klasse. Vertegenwoordigt een verzameling van Resource-objecten"
type: docs
weight: 1770
url: /nl/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Vertegenwoordigt een verzameling van [`Resource`](../resource/) objecten.

```csharp
public class ResourceCollection : IList<Resource>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Haalt het aantal elementen op dat in de ResourceCollection zit. Alleen-lezen Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Haalt het bovenliggende project op van het ResourceCollection-object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Voegt een nieuwe resource toe op de opgegeven positie van een projectresourceverzameling. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Direct wissen wordt niet ondersteund, deze methode gooit alleen NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Retourneert een resource met de opgegeven id. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Retourneert een resource met de opgegeven Uid. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Dit is de stub-implementatie van de Remove-methode van ICollection, die alleen NotSupportedException gooit. |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Converteert het ResourceCollection-object naar een lijst van [`Resource`](../resource/) objecten. |

## Voorbeelden

Toont hoe te werken met resourceverzamelingen.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// voeg lege resource toe
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// voeg resource met een naam toe
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// voeg resource toe vóór de resource met opgegeven ID
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// haal resource op op basis van id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// resourceverzamelingen ondersteunen de Clear-bewerking niet
// project.Resources.Clear();
// gebruik het volgende codevoorbeeld in plaats daarvan
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Zie ook

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


