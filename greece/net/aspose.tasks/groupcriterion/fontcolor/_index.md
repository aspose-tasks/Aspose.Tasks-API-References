---
title: "GroupCriterion.FontColor"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GroupCriterion ιδιότητα. Λαμβάνει ή ορίζει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε έναν ορισμό ομάδας"
type: docs
weight: 60
url: /el/net/aspose.tasks/groupcriterion/fontcolor/
---
## GroupCriterion.FontColor property

Λαμβάνει ή ορίζει το χρώμα της γραμματοσειράς για ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας.

```csharp
public Color FontColor { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες ενός κριτηρίου ομάδας.

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

// Διαβάστε το υπόβαθρο του προτύπου του κριτηρίου.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Δείτε επίσης

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


