---
title: "ResourceCollection.Clear"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceCollection. La suppression directe n'est pas prise en charge, cette méthode lève simplement NotSupportedException"
type: docs
weight: 50
url: /fr/net/aspose.tasks/resourcecollection/clear/
---
## ResourceCollection.Clear method

Le nettoyage direct n'est pas pris en charge, cette méthode lève simplement NotSupportedException.

```csharp
public void Clear()
```

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

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


