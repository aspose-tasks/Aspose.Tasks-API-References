---
title: "Filter.op_Inequality"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Filter. Retourne une valeur indiquant si cette instance n'est pas égale à un objet spécifié."
type: docs
weight: 150
url: /fr/net/aspose.tasks/filter/op_inequality/
---
## Filter Inequality operator

Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

```csharp
public static bool operator !=(Filter a, Filter b)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| a | Filter | Le premier filtre. |
| b | Filter | Le deuxième filtre. |

### Valeur de retour

une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

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


