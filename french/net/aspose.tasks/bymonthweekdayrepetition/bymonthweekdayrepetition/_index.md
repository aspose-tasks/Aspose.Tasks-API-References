---
title: "ByMonthWeekDayRepetition.ByMonthWeekDayRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur ByMonthWeekDayRepetition. Initialise une nouvelle instance de la classe ByMonthWeekDayRepetition"
type: docs
weight: 10
url: /fr/net/aspose.tasks/bymonthweekdayrepetition/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition constructor

Initialise une nouvelle instance de la classe [`ByMonthWeekDayRepetition`](../).

```csharp
public ByMonthWeekDayRepetition()
```

## Exemples

Montre comment travailler avec les répétitions de jours de semaine mensuels lors de la création de nouvelles tâches récurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


