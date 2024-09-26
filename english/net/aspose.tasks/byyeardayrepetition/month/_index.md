---
title: ByYearDayRepetition.Month
second_title: Aspose.Tasks for .NET API Reference
description: ByYearDayRepetition property. Gets or sets a month on which the task must be recurring
type: docs
weight: 30
url: /net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

Gets or sets a month on which the task must be recurring.

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


