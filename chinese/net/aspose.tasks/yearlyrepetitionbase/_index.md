---
title: "类 YearlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.YearlyRepetitionBase 类。表示 年度 天 位置 的 基础 模式"
type: docs
weight: 3700
url: /zh/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

表示年度日期位置的基础模式。

```csharp
public abstract class YearlyRepetitionBase
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


