---
title: ByYearDayRepetition.DayPosition
second_title: Aspose.Tasks for .NET API Reference
description: ByYearDayRepetition property. Gets or sets a position of day in a month on which the task must be recurring
type: docs
weight: 20
url: /net/aspose.tasks/byyeardayrepetition/dayposition/
---
## ByYearDayRepetition.DayPosition property

Gets or sets a position of day in a month on which the task must be recurring.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


