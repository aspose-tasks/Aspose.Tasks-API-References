---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur ByYearWeekDayRepetition. Initialise une nouvelle instance de la classe ByYearWeekDayRepetition"
type: docs
weight: 10
url: /fr/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

Initialise une nouvelle instance de la classe [`ByYearWeekDayRepetition`](../).

```csharp
public ByYearWeekDayRepetition()
```

## Exemples

Montre comment travailler avec les répétitions de jours de la semaine sur une année lors de la création de nouvelles tâches récurrentes.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


