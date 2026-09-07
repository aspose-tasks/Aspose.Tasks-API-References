---
title: "Tsk.Cost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για μια εργασία, βασισμένο στα ήδη προκύψαντα κόστη για την εργασία που εκτελείται από τους ανατεθειμένους πόρους, επιπλέον των κόστους που έχουν προγραμματιστεί για την εναπομείνασα εργασία."
type: docs
weight: 230
url: /el/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

Το συνολικό προγραμματισμένο ή προβλεπόμενο κόστος για μια εργασία, βασισμένο στα κόστη που έχουν ήδη προκύψει για την εργασία που εκτελείται από τους πόρους που έχουν ανατεθεί στις εργασίες, καθώς και στα κόστη που έχουν προγραμματιστεί για την υπόλοιπη εργασία.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


