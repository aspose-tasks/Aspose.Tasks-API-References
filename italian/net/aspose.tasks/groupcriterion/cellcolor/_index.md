---
title: "GroupCriterion.CellColor"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GroupCriterion proprietà. Ottiene o imposta il colore di sfondo della cella per un campo usato come criterio in una definizione di gruppo"
type: docs
weight: 30
url: /it/net/aspose.tasks/groupcriterion/cellcolor/
---
## GroupCriterion.CellColor property

Ottiene o imposta il colore dello sfondo della cella per un campo utilizzato come criterio in una definizione di gruppo.

```csharp
public Color CellColor { get; set; }
```

## Esempi

Mostra come leggere le proprietà di un criterio di gruppo.

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

// leggi il modello di sfondo del criterio
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

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


