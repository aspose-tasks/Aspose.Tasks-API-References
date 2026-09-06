---
title: "RecurrenceRangeBase.Start"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété RecurrenceRangeBase. Obtient ou définit la date de début de la plage de récurrence de la tâche récurrente"
type: docs
weight: 10
url: /fr/net/aspose.tasks/recurrencerangebase/start/
---
## RecurrenceRangeBase.Start property

Obtient ou définit la date de début de la plage de récurrence de la tâche récurrente.

```csharp
public DateTime Start { get; set; }
```

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

* class [RecurrenceRangeBase](../)
* namespace [Aspose.Tasks](../../recurrencerangebase/)
* assembly [Aspose.Tasks](../../../)


