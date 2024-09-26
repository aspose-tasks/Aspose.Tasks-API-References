---
title: MonthlyRepetitionBase.RepetitionInterval
second_title: Aspose.Tasks for .NET API Reference
description: MonthlyRepetitionBase property. Gets or sets a number of month which represents the interval in months between occurrences
type: docs
weight: 10
url: /net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

Gets or sets a number of month which represents the interval in months between occurrences.

```csharp
public int RepetitionInterval { get; set; }
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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


