---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraProjectProperties. Λαμβάνει πίνακα με τα baseline έργα του τρέχοντος έργου. Εφαρμόζεται σε έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενα baselines."
type: docs
weight: 10
url: /el/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Λαμβάνει έναν πίνακα των έργων βάσης του τρέχοντος έργου. Εφαρμόζεται σε έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενες βάσεις.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


