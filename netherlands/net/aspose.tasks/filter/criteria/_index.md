---
title: "Filter.Criteria"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Filter-eigenschap. Haalt de criteria op of stelt de criteria in waaraan taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave."
type: docs
weight: 20
url: /nl/net/aspose.tasks/filter/criteria/
---
## Filter.Criteria property

Haalt de criteria op of stelt ze in die taken of resources moeten voldoen om weergegeven te worden in de MSP-weergave.

```csharp
public FilterCriteria Criteria { get; set; }
```

## Voorbeelden

Toont hoe taakfilters te lezen.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### Zie ook

* class [FilterCriteria](../../filtercriteria/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


