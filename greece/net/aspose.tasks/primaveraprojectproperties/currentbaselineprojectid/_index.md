---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraProjectProperties. Λαμβάνει το Id του τρέχοντος baseline έργου. Ισχύει για έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενα baselines"
type: docs
weight: 40
url: /el/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Λαμβάνει το Id του τρέχοντος έργου βάσης. Εφαρμόζεται σε έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενες βάσεις.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML και να εξετάσετε τα δεδομένα baseline του έργου.

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### Δείτε επίσης

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


