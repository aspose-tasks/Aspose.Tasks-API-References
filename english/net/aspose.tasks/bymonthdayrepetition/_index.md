---
title: Class ByMonthDayRepetition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ByMonthDayRepetition class. Represents a pattern which is based on the absolute position of a day in a month
type: docs
weight: 170
url: /net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Represents a pattern which is based on the absolute position of a day in a month.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Initializes a new instance of the `ByMonthDayRepetition` class. |

## Properties

| Name | Description |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Gets or sets a position of a day in a month on which the task must be recurring. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Gets or sets a number of month which represents the interval in months between occurrences. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


