---
title: "Filter.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Filter. Retourne une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié"
type: docs
weight: 100
url: /fr/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié.

```csharp
public bool Equals(Filter other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| autre | Filter | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie vrai si cette instance est égale à l'objet AssignmentBaseline spécifié ; sinon, faux.

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

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à l'objet AssignmentBaseline spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | l'objet AssignmentBaseline spécifié à comparer avec cette instance. |

### Valeur de retour

renvoie vrai si cette instance est égale à l'objet AssignmentBaseline spécifié ; sinon, faux.

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


