---
title: Enum Month
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Month enum. Specifies the month
type: docs
weight: 1020
url: /net/aspose.tasks/month/
---
## Month enumeration

Specifies the month.

```csharp
public enum Month
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates the value was not defined in original project file. |
| January | `0` | Indicates January month. |
| February | `1` | Indicates February month. |
| March | `2` | Indicates March month. |
| April | `3` | Indicates April month. |
| May | `4` | Indicates May month. |
| June | `5` | Indicates June month. |
| July | `6` | Indicates July month. |
| August | `7` | Indicates August month. |
| September | `8` | Indicates September month. |
| October | `9` | Indicates October month. |
| November | `10` | Indicates November month. |
| December | `11` | Indicates December month. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

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


