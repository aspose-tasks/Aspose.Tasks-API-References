---
title: "GroupCriterion.Pattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GroupCriterion-eigenschap. Haalt op of stelt het patroon van de cel in voor een veld dat wordt gebruikt als criterium in een groepsdefinitie."
type: docs
weight: 90
url: /nl/net/aspose.tasks/groupcriterion/pattern/
---
## GroupCriterion.Pattern property

Haalt het patroon van de cel op of stelt het in voor een veld dat wordt gebruikt als criterium in een groepsdefinitie.

```csharp
public BackgroundPattern Pattern { get; set; }
```

## Voorbeelden

Toont hoe de eigenschappen van een groepscriterium gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// lees het achtergrondpatroon van het criterium
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Zie ook

* enum [BackgroundPattern](../../backgroundpattern/)
* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


