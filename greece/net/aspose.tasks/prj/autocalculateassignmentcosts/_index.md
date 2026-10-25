---
title: "Prj.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία των αναθέσεων και τις τιμές των πόρων"
type: docs
weight: 60
url: /el/net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

Καθορίζει εάν το κόστος ανάθεσης και το υπόλοιπο κόστος πρέπει να υπολογίζονται αυτόματα χρησιμοποιώντας την εργασία και τις τιμές πόρων της ανάθεσης.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

## Παραδείγματα

Δείχνει πώς να απενεργοποιήσετε τον αυτόματο υπολογισμό του κόστους της ανάθεσης και να ορίσετε το κόστος της ανάθεσης ρητά.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


