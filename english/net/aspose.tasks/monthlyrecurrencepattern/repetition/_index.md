---
title: MonthlyRecurrencePattern.Repetition
second_title: Aspose.Tasks for .NET API Reference
description: MonthlyRecurrencePattern property. Gets or sets the recurring repetition pattern
type: docs
weight: 20
url: /net/aspose.tasks/monthlyrecurrencepattern/repetition/
---
## MonthlyRecurrencePattern.Repetition property

Gets or sets the recurring repetition pattern.

```csharp
public MonthlyRepetitionBase Repetition { get; set; }
```

## Examples

Shows how to work with monthly recurrence pattern repetitions while create recurring tasks.

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

* class [MonthlyRepetitionBase](../../monthlyrepetitionbase/)
* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


