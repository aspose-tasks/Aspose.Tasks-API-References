---
title: Class YearlyRecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.YearlyRecurrencePattern class. Represents the set of parameters are used to create a yearly recurring task in a project
type: docs
weight: 3610
url: /net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Represents the set of parameters are used to create a yearly recurring task in a project.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Name | Description |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Initializes a new instance of the `YearlyRecurrencePattern` class. |

## Properties

| Name | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Gets or sets the recurrence range. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Gets or sets the recurring position pattern. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


