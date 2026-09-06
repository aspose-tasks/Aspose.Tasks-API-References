---
title: "Classe Filter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Filter. Représente un filtre dans Project"
type: docs
weight: 600
url: /fr/net/aspose.tasks/filter/
---
## Filter class

Représente un filtre dans Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Filter](filter/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Obtient ou définit les critères que les tâches ou ressources doivent satisfaire pour être affichés dans la vue MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Obtient le type du filtre. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Obtient l'index d'un objet `Filter` dans l'objet contenant les filtres. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Obtient ou définit le nom d'un objet Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Obtient ou définit une valeur indiquant si le projet affiche le nom du filtre dans la liste déroulante Filter de l'onglet View du Ruban. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Obtient ou définit une valeur indiquant si les lignes de résumé associées sont affichées pour le filtre. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Obtient l'identifiant unique d'un filtre. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Compare cette instance à l'instance spécifiée de la classe `Filter` et renvoie une indication de leur ordre relatif. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Renvoie une valeur de code de hachage pour le filtre. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Renvoie une valeur indiquant si cette instance est supérieure à un objet spécifié. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Renvoie une valeur indiquant si cette instance est supérieure ou égale à un objet spécifié. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Renvoie une valeur indiquant si cette instance est inférieure à un objet spécifié. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Renvoie une valeur indiquant si cette instance est inférieure ou égale à un objet spécifié. |

## Exemples

Montre comment travailler avec les filtres.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// vérifier les filtres de ressources
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


