---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Filter-methode. Vergelijkt deze instantie met de opgegeven instantie van de Filter-klasse en retourneert een indicatie van hun relatieve volgorde"
type: docs
weight: 90
url: /nl/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Vergelijkt deze instantie met de opgegeven instantie van de [`Filter`](../)-klasse en retourneert een indicatie van hun relatieve volgorde.

```csharp
public int CompareTo(Filter other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | Filter | de opgegeven instantie van de [`Filter`](../)-klasse om te vergelijken met dit object. |

### Retourwaarde

een indicatie van hun relatieve volgorde.

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


