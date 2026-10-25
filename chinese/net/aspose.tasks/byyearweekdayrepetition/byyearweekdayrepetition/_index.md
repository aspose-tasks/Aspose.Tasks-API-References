---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ByYearWeekDayRepetition 构造函数。初始化 ByYearWeekDayRepetition 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

初始化 [`ByYearWeekDayRepetition`](../) 类的新实例。

```csharp
public ByYearWeekDayRepetition()
```

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

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


