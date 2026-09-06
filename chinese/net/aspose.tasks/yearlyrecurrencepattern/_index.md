---
title: "类 YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.YearlyRecurrencePattern 类。表示用于在项目中创建年度循环任务的一组参数"
type: docs
weight: 3690
url: /zh/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

表示用于在项目中创建年度循环任务的参数集合。

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | 初始化 `YearlyRecurrencePattern` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 获取或设置循环范围。 |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | 获取或设置循环位置模式。 |

## 示例

展示在创建循环任务时如何使用年度循环模式。

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

### 另见

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


