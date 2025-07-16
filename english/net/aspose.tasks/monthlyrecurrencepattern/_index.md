---
title: Class MonthlyRecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MonthlyRecurrencePattern class. Represents the set of parameters are used to create a monthly recurring task in a project
type: docs
weight: 1060
url: /net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Represents the set of parameters are used to create a monthly recurring task in a project.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Name | Description |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Initializes a new instance of the `MonthlyRecurrencePattern` class. |

## Properties

| Name | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Gets or sets the recurrence range. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Gets or sets the recurring repetition pattern. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


