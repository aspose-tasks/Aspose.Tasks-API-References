---
title: ByYearWeekDayRepetition.Month
second_title: Aspose.Tasks for .NET API Reference
description: ByYearWeekDayRepetition property. Gets or sets a month on which the task must be recurring
type: docs
weight: 20
url: /net/aspose.tasks/byyearweekdayrepetition/month/
---
## ByYearWeekDayRepetition.Month property

Gets or sets a month on which the task must be recurring.

```csharp
public Month Month { get; set; }
```

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

* enum [Month](../../month/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


