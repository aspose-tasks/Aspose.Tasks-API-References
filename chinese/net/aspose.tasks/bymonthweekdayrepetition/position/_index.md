---
title: "ByMonthWeekDayRepetition.Position"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ByMonthWeekDayRepetition 属性。获取或设置任务必须在其重复的月份中星期几的位置"
type: docs
weight: 20
url: /zh/net/aspose.tasks/bymonthweekdayrepetition/position/
---
## ByMonthWeekDayRepetition.Position property

获取或设置任务必须重复的月份中工作日的位置。

```csharp
public OrdinalNumber Position { get; set; }
```

## 示例

展示在创建新循环任务时如何使用月份工作日重复。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


