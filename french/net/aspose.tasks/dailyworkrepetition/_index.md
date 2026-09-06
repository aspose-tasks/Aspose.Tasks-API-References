---
title: "Classe DailyWorkRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.DailyWorkRepetition. Représente une classe pour les répétitions dans le modèle de récurrence quotidien basé sur les jours ouvrés"
type: docs
weight: 420
url: /fr/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Représente une classe pour les répétitions dans un modèle de récurrence quotidien basé sur les jours ouvrés.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Initialise une nouvelle instance de la classe `DailyWorkRepetition`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Obtient ou définit un nombre de jours qui représente l'intervalle en jours entre les occurrences. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


