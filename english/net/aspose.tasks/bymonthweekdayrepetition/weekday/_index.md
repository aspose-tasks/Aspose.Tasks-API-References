---
title: ByMonthWeekDayRepetition.WeekDay
second_title: Aspose.Tasks for .NET API Reference
description: ByMonthWeekDayRepetition property. Gets or sets a type of weekday on which the task must be recurring
type: docs
weight: 30
url: /net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

Gets or sets a type of weekday on which the task must be recurring.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## Examples

Shows how to work with month weekday repetitions while create a new recurring tasks.

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

### See Also

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


