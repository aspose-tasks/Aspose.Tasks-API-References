---
title: "Tsk.ConstraintDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η συγκεκριμένη ημερομηνία που σχετίζεται με τον τύπο περιορισμού"
type: docs
weight: 200
url: /el/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

Η συγκεκριμένη ημερομηνία που σχετίζεται με τον τύπο περιορισμού.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Παραδείγματα

Δείχνει πώς να λάβετε/ορίσετε έναν περιορισμό για μια εργασία.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Ορίστε τον περιορισμό Όσο Αργά Όσο Είναι Δυνατό για την εργασία με Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


