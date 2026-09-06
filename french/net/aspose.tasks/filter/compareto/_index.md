---
title: "Filter.CompareTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Filter. Compare cette instance à l'instance spécifiée de la classe Filter et renvoie une indication de leur ordre relatif"
type: docs
weight: 90
url: /fr/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Compare cette instance à l'instance spécifiée de la classe [`Filter`](../) et renvoie une indication de leur ordre relatif.

```csharp
public int CompareTo(Filter other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | Filter | l'instance spécifiée de la classe [`Filter`](../) à comparer à cet objet. |

### Valeur de retour

une indication de leur ordre relatif.

## Exemples

Montre comment vérifier l'égalité du filtre.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// l'égalité des filtres est vérifiée par rapport à l'UID du filtre.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Voir aussi

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


