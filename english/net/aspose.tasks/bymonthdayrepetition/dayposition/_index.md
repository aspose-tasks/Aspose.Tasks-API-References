---
title: ByMonthDayRepetition.DayPosition
second_title: Aspose.Tasks for .NET API Reference
description: ByMonthDayRepetition property. Gets or sets a position of a day in a month on which the task must be recurring
type: docs
weight: 20
url: /net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

Gets or sets a position of a day in a month on which the task must be recurring.

```csharp
public int DayPosition { get; set; }
```

## Examples

Shows how to work with month day repetitions while create a new recurring tasks.

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

### See Also

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


