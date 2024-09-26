---
title: YearlyRecurrencePattern.YearlyRecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: YearlyRecurrencePattern constructor. Initializes a new instance of the YearlyRecurrencePattern class
type: docs
weight: 10
url: /net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Initializes a new instance of the [`YearlyRecurrencePattern`](../) class.

```csharp
public YearlyRecurrencePattern()
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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


