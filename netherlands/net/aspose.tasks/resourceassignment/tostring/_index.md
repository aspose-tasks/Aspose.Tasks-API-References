---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment methode. Retourneert een korte tekenreeksrepresentatie van de instantie van de ResourceAssignment-klasse. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen."
type: docs
weight: 790
url: /nl/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Retourneert een korte tekenreeksrepresentatie van de instantie van de [`ResourceAssignment`](../) klasse. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

```csharp
public override string ToString()
```

### Retourwaarde

korte tekenreeks die een toewijzingsobject vertegenwoordigt.

## Voorbeelden

Toont hoe je algemene toewijzingsinformatie afdrukt.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // toon de toewijzingen van de taak
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


