---
title: "Tsk.ConstraintType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Παρέχει επιλογές για τον τύπο περιορισμού που μπορεί να εφαρμοστεί για τον προγραμματισμό μιας εργασίας"
type: docs
weight: 210
url: /el/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

Παρέχει επιλογές για τον τύπο περιορισμού που μπορεί να εφαρμοστεί για τον προγραμματισμό ενός έργου.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
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
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


