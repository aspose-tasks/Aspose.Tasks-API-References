---
title: "Tsk.CostVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διαφορά μεταξύ του κόστους βάσης και του συνολικού κόστους για έναν πόρο ή ανάθεση εργασίας."
type: docs
weight: 240
url: /el/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

Η διαφορά μεταξύ του αρχικού κόστους και του συνολικού κόστους για μια εργασία, πόρο ή ανάθεση.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


