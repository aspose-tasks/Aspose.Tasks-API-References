---
title: "Tsk.ConstraintDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date spécifique associée au type de contrainte"
type: docs
weight: 200
url: /fr/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

La date spécifique associée au type de contrainte.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Exemples

Montre comment obtenir/définir une contrainte pour une tâche.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Définir la contrainte Au Plus Tard Possible pour la tâche avec Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


