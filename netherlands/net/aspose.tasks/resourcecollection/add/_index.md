---
title: "ResourceCollection.Add"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceCollection‑methode. Voegt een nieuwe resource toe op de laatste positie van een project‑resources‑collectie"
type: docs
weight: 40
url: /nl/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling.

```csharp
public Resource Add()
```

### Retourwaarde

Bron toegevoegd.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_1}

Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling.

```csharp
public Resource Add(string resourceName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| resourceName | String | Naam van een bron. |

### Retourwaarde

Bron toegevoegd.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_2}

Voegt een nieuwe resource toe op de opgegeven positie van een projectresourceverzameling.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| resourceName | String | Naam van een bron. |
| beforeResourceId | Int32 | Positie van de vorige bron in een projectbronnenverzameling. |

### Retourwaarde

Bron toegevoegd.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


