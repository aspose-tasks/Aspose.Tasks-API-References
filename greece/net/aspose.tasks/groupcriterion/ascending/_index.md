---
title: "GroupCriterion.Ascending"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GroupCriterion. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας ταξινομείται σε αύξουσα σειρά. Ψευδής εάν το πεδίο ταξινομείται σε φθίνουσα σειρά."
type: docs
weight: 20
url: /el/net/aspose.tasks/groupcriterion/ascending/
---
## GroupCriterion.Ascending property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένα πεδίο που χρησιμοποιείται ως κριτήριο σε ορισμό ομάδας είναι ταξινομημένο σε αύξουσα σειρά. Ψευδές εάν το πεδίο είναι ταξινομημένο σε φθίνουσα σειρά.

```csharp
public bool Ascending { get; set; }
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


