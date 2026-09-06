---
title: "Classe ResourceCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ResourceCollection. Représente une collection d'objets Resource"
type: docs
weight: 1770
url: /fr/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Représente une collection d'objets [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Obtient le nombre d'éléments contenus dans le ResourceCollection. Int32 en lecture seule. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Obtient le projet parent de l'objet ResourceCollection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Ajoute une nouvelle ressource à la dernière position d'une collection de ressources du projet. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Ajoute une nouvelle ressource à la dernière position d'une collection de ressources du projet. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Ajoute une nouvelle ressource à la position spécifiée d'une collection de ressources du projet. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Le nettoyage direct n'est pas pris en charge, cette méthode lève simplement NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Renvoie une ressource avec l'ID spécifié. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Renvoie une ressource avec le Uid spécifié. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Ceci est l'implémentation factice de la méthode Remove de ICollection, qui ne lance que NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Convertit l'objet ResourceCollection en une liste d'objets [`Resource`](../resource/). |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


