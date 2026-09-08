---
title: "Filter.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Filter-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object."
type: docs
weight: 100
url: /nl/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object.

```csharp
public bool Equals(Filter other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | Filter | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als deze instantie gelijk is aan het opgegeven AssignmentBaseline-object; anders false.

## Voorbeelden

Toont hoe de filtergelijkheid te controleren.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// De gelijkheid van filters wordt gecontroleerd tegen de UID van de filter.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Zie ook

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven AssignmentBaseline-object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als deze instantie gelijk is aan het opgegeven AssignmentBaseline-object; anders false.

## Voorbeelden

Toont hoe de filtergelijkheid te controleren.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// De gelijkheid van filters wordt gecontroleerd tegen de UID van de filter.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Zie ook

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


