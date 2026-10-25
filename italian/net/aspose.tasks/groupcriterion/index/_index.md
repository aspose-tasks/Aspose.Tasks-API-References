---
title: "GroupCriterion.Index"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GroupCriterion proprietà. Ottiene l'indice di un oggetto GroupCriterion nella collezione GroupCriterionCollection contenente"
type: docs
weight: 90
url: /it/net/aspose.tasks/groupcriterion/index/
---
## GroupCriterion.Index property

Ottiene l'indice di un oggetto [`GroupCriterion`](../) nella collezione [`GroupCriterionCollection`](../../groupcriterioncollection/) contenente.

```csharp
public int Index { get; }
```

## Esempi

Mostra come lavorare con un criterio di gruppo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Index: " + criterion.Index);
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// leggi il modello di sfondo del criterio
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

if (group == criterion.ParentGroup)
{
    Console.WriteLine("Parent Group is equal to task Group.");
}

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Vedi anche

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


