---
title: Class ByYearWeekDayRepetition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ByYearWeekDayRepetition class. Represents a pattern which is based on position of a weekday in a month
type: docs
weight: 200
url: /net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Represents a pattern which is based on position of a weekday in a month.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Initializes a new instance of the `ByYearWeekDayRepetition` class. |

## Properties

| Name | Description |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Gets or sets a month on which the task must be recurring. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Gets or sets a position of the day in a week of a month on which the task must be recurring. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Gets or sets a type of week day on which the task must be recurring. |

## Examples

Shows how to work with year weekday repetitions while create a new recurring tasks.

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

### See Also

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


