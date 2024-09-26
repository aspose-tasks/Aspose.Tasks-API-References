---
title: Class ByMonthWeekDayRepetition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ByMonthWeekDayRepetition class. Represents a pattern which is based on the position of weekday in a month
type: docs
weight: 180
url: /net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Represents a pattern which is based on the position of weekday in a month.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Initializes a new instance of the `ByMonthWeekDayRepetition` class. |

## Properties

| Name | Description |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Gets or sets a position of weekday in a month on which the task must be recurring. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Gets or sets a number of month which represents the interval in months between occurrences. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Gets or sets a type of weekday on which the task must be recurring. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


