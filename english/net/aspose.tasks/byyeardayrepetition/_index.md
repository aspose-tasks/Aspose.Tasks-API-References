---
title: Class ByYearDayRepetition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ByYearDayRepetition class. Represents a pattern which is based on the absolute position of a day in a month
type: docs
weight: 190
url: /net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Represents a pattern which is based on the absolute position of a day in a month.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Constructors

| Name | Description |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Initializes a new instance of the `ByYearDayRepetition` class. |

## Properties

| Name | Description |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Gets or sets a position of day in a month on which the task must be recurring. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Gets or sets a month on which the task must be recurring. |

## Examples

Shows how to work with year day repetitions while create a new recurring tasks.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


