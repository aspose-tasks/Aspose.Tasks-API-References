---
title: "类 ByMonthWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ByMonthWeekDayRepetition 类。表示基于月份中工作日位置的模式"
type: docs
weight: 180
url: /zh/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

表示基于月份中星期几位置的模式。

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | 初始化 `ByMonthWeekDayRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | 获取或设置任务必须重复的月份中工作日的位置。 |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示两次出现之间间隔月份数的月份数。 |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | 获取或设置任务必须重复的工作日类型。 |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


