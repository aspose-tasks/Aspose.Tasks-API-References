---
title: "ByYearDayRepetition.Month"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ByYearDayRepetition 属性。获取或设置任务必须重复的月份"
type: docs
weight: 30
url: /zh/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

获取或设置任务必须重复的月份。

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


