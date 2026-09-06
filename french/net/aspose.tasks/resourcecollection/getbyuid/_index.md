---
title: "ResourceCollection.GetByUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceCollection. Retourne une ressource avec l'Uid spécifié"
type: docs
weight: 70
url: /fr/net/aspose.tasks/resourcecollection/getbyuid/
---
## ResourceCollection.GetByUid method

Renvoie une ressource avec le Uid spécifié.

```csharp
public Resource GetByUid(int uid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| uid | Int32 | L'uid spécifié. |

### Valeur de retour

Ressource avec l'uid spécifié si présente ; sinon, null.

## Remarques

Complexité O(1).

## Exemples

Montre comment travailler avec des collections de ressources.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// ajouter une ressource vide
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// ajouter une ressource avec un nom
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// ajouter une ressource avant la ressource avec l'ID spécifié
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// obtenir la ressource par ID
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// les collections de ressources ne prennent pas en charge l'opération Clear
// project.Resources.Clear();
// utilisez l'exemple de code suivant à la place
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Voir aussi

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


