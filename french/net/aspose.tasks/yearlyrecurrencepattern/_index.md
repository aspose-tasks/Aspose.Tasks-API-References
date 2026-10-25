---
title: "Classe YearlyRecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.YearlyRecurrencePattern class. Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente annuelle dans un projet"
type: docs
weight: 3690
url: /fr/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente annuelle dans un projet.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Initialise une nouvelle instance de la classe `YearlyRecurrencePattern`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtient ou définit la plage de récurrence. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Obtient ou définit le modèle de position récurrente. |

## Exemples

Montre comment travailler avec les modèles de récurrence annuels lors de la création de tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


