---
title: "类 ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ByYearDayRepetition 类。表示基于月份中某一天的绝对位置的模式。"
type: docs
weight: 190
url: /zh/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

表示基于月份中某天绝对位置的模式。

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | 初始化 `ByYearDayRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | 获取或设置任务必须循环的月份中某一天的位置。 |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | 获取或设置任务必须重复的月份。 |

## 示例

展示在创建新循环任务时如何使用年度天重复。

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

### 另见

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


