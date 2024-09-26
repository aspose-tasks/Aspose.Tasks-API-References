---
title: YearlyRecurrencePattern.Repetition
second_title: Aspose.Tasks for .NET API Reference
description: YearlyRecurrencePattern property. Gets or sets the recurring position pattern
type: docs
weight: 20
url: /net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

Gets or sets the recurring position pattern.

```csharp
public YearlyRepetitionBase Repetition { get; set; }
```

## Examples

Shows how to work with year year recurrence patterns while creating recurring tasks.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


