---
title: "Filter.op_LessThan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Filter-methode. Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object"
type: docs
weight: 160
url: /nl/net/aspose.tasks/filter/op_lessthan/
---
## Filter LessThan operator

Retourneert een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object.

```csharp
public static bool operator <(Filter a, Filter b)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| een | Filter | De eerste filter. |
| b | Filter | De tweede filter. |

### Retourwaarde

een waarde die aangeeft of deze instantie kleiner is dan een opgegeven object

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


