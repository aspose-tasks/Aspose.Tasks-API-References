---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur YearlyRecurrencePattern. Initialise une nouvelle instance de la classe YearlyRecurrencePattern"
type: docs
weight: 10
url: /fr/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Initialise une nouvelle instance de la classe [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
```

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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


