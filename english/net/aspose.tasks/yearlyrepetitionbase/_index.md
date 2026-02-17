---
title: Class YearlyRepetitionBase
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.YearlyRepetitionBase class. Represents a base pattern for yearly day position
type: docs
weight: 3680
url: /net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

Represents a base pattern for yearly day position.

```csharp
public abstract class YearlyRepetitionBase
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


