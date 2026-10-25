---
title: "Tsk.FixedCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Εμφανίζει τυχόν έξοδα εργασίας που δεν αφορούν πόρους"
type: docs
weight: 430
url: /el/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

Εμφανίζει τυχόν έξοδα μη-πόρων για την εργασία.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τα κόστη εργασίας.

```csharp
var project = new Project();

// Προσθέστε εργασία και ορίστε κόστος
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Εμφανίστε ιδιότητες σχετικές με το κόστος της εργασίας
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


