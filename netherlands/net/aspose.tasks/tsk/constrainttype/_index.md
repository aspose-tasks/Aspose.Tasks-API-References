---
title: "Tsk.ConstraintType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Biedt keuzes voor het type beperking dat kan worden toegepast bij het plannen van een taak"
type: docs
weight: 210
url: /nl/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

Biedt keuzes voor het type beperking dat kan worden toegepast bij het plannen van een taak.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## Voorbeelden

Toont hoe een constraint voor een taak te krijgen/instellen.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Stel constraint As Late As Possible in voor taak met Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


