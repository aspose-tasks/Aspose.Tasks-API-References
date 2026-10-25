---
title: "类 ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ByYearWeekDayRepetition 类。表示基于月份中某个工作日位置的模式"
type: docs
weight: 200
url: /zh/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

表示基于月份中某个星期几位置的模式。

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | 初始化 `ByYearWeekDayRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | 获取或设置任务必须重复的月份。 |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | 获取或设置任务必须重复的月份中某周的天的位置。 |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | 获取或设置任务必须重复的星期几类型。 |

## 示例

展示在创建新循环任务时如何使用年度星期重复。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


