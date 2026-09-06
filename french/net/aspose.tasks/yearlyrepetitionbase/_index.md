---
title: "Classe YearlyRepetitionBase"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.YearlyRepetitionBase. Représente un modèle de base pour la position de jour annuelle."
type: docs
weight: 3700
url: /fr/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

Représente un modèle de base pour la position du jour annuel.

```csharp
public abstract class YearlyRepetitionBase
```

## Exemples

Montre comment travailler avec les répétitions de jour de l'année lors de la création de nouvelles tâches récurrentes.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


