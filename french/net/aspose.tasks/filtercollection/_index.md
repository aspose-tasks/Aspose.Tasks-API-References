---
title: "Classe FilterCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.FilterCollection. Contient une liste d'objets Filter. Implémente l'interface ICollectionFilter."
type: docs
weight: 610
url: /fr/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Contient une liste d'objets [`Filter`](../filter/). Implémente l'interface ICollection&lt;Filter&gt;.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Convertit une collection de filtres en une liste d'objets [`Filter`](../filter/). |

## Exemples

Montre comment travailler avec des collections de filtres.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// itérer sur les filtres de tâches
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// itérer sur les filtres de ressources
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// effacer les filtres d'un autre projet
otherProject.TaskFilters.Clear();

// copier les filtres vers un autre projet
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// ajouter un filtre de tâche personnalisé
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// supprimer tous les filtres
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Voir aussi

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


