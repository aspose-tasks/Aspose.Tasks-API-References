---
title: "FilterCollection.Add"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode FilterCollection. Ajoute l'élément spécifié à cette collection."
type: docs
weight: 30
url: /fr/net/aspose.tasks/filtercollection/add/
---
## FilterCollection.Add method

Ajoute l'élément spécifié à cette collection.

```csharp
public void Add(Filter item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | Filter | l'élément spécifié à ajouter à cette collection. |

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


