---
title: "Classe MonthlyRecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.MonthlyRecurrencePattern. Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente mensuelle dans un projet"
type: docs
weight: 1080
url: /fr/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente mensuelle dans un projet.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Initialise une nouvelle instance de la classe `MonthlyRecurrencePattern`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtient ou définit la plage de récurrence. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Obtient ou définit le modèle de répétition récurrent. |

## Exemples

Montre comment travailler avec les répétitions de motif de récurrence mensuelle lors de la création de tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


