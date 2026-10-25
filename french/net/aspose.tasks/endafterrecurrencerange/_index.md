---
title: "Classe EndAfterRecurrenceRange"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.EndAfterRecurrenceRange. Représente la plage de récurrence d'une tâche récurrente qui est limitée par le nombre d'occurrences"
type: docs
weight: 500
url: /fr/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Représente la plage de récurrence d'une tâche récurrente limitée par le nombre d'occurrences.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Initialise une nouvelle instance de la classe `EndAfterRecurrenceRange`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Obtient ou définit le nombre d'occurrences qui limite la plage de récurrence de la tâche récurrente. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Obtient ou définit la date de début de la plage de récurrence de la tâche récurrente. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


