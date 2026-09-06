---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "YearlyRecurrencePattern 构造函数。初始化 YearlyRecurrencePattern 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

初始化 [`YearlyRecurrencePattern`](../) 类的新实例。

```csharp
public YearlyRecurrencePattern()
```

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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


