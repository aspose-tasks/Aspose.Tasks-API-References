---
title: "Classe RecurrencePatternBase"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.RecurrencePatternBase. Représente la classe de base du modèle de récurrence"
type: docs
weight: 1700
url: /fr/net/aspose.tasks/recurrencepatternbase/
---
## RecurrencePatternBase class

Représente la classe de base du modèle de récurrence.

```csharp
public abstract class RecurrencePatternBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtient ou définit la plage de récurrence. |

## Exemples

Montre comment travailler avec les répétitions du modèle de répétition quotidienne lors de la création de tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// continuer à travailler avec le projet...
// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


