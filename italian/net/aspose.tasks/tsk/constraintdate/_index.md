---
title: "Tsk.ConstraintDate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data specifica associata al tipo di vincolo"
type: docs
weight: 200
url: /it/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

La data specifica associata al tipo di vincolo.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Esempi

Mostra come ottenere/impostare un vincolo per un'attività.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Imposta il vincolo Il più tardi possibile per l'attività con Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


