---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété DailyRepetitionBase. Obtient ou définit un nombre de jours qui représente l'intervalle en jours entre les occurrences"
type: docs
weight: 10
url: /fr/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

Obtient ou définit un nombre de jours qui représente l'intervalle en jours entre les occurrences.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


