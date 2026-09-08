---
title: "Klasse Filter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Filter-klasse. Vertegenwoordigt een filter in Project"
type: docs
weight: 600
url: /nl/net/aspose.tasks/filter/
---
## Filter class

Stelt een filter in Project voor.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Filter](filter/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Haalt de criteria op of stelt ze in die taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Haalt het type van het filter op. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Haalt de index op van een `Filter`-object in het object dat de Filters bevat. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Haalt de naam van een Filter-object op of stelt deze in. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of het project de filternaam toont in de Filter‑keuzelijst op het tabblad Weergave van het lint. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of gerelateerde samenvattingsrijen worden weergegeven voor het filter. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Haalt de unieke identifier van een filter op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Vergelijkt deze instantie met de opgegeven instantie van de `Filter`-klasse en retourneert een indicatie van hun relatieve volgorde. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Retourneert een hashcode-waarde voor het filter. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Retourneert een waarde die aangeeft of deze instantie groter is dan een opgegeven object. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Retourneert een waarde die aangeeft of deze instantie groter dan of gelijk aan een opgegeven object is. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Retourneert een waarde die aangeeft of deze instantie kleiner dan of gelijk aan een opgegeven object is. |

## Voorbeelden

Toont hoe je met filters werkt.

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

// controleer resource-filters
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


