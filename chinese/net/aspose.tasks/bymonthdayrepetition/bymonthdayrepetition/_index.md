---
title: "ByMonthDayRepetition.ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ByMonthDayRepetition 构造函数。初始化 ByMonthDayRepetition 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/bymonthdayrepetition/bymonthdayrepetition/
---
## ByMonthDayRepetition constructor

初始化 [`ByMonthDayRepetition`](../) 类的新实例。

```csharp
public ByMonthDayRepetition()
```

## 示例

展示如何在创建新循环任务时使用月份天数重复。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


