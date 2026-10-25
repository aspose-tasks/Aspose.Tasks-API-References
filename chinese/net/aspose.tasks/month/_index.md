---
title: "枚举 Month"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Month 枚举。指定月份。"
type: docs
weight: 1040
url: /zh/net/aspose.tasks/month/
---
## Month enumeration

指定月份。

```csharp
public enum Month
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示该值未在原始项目文件中定义。 |
| January | `0` | 指示一月。 |
| February | `1` | 指示二月。 |
| March | `2` | 指示三月。 |
| April | `3` | 指示四月。 |
| May | `4` | 指示五月。 |
| June | `5` | 指示六月。 |
| July | `6` | 指示七月。 |
| August | `7` | 指示八月。 |
| September | `8` | 指示九月。 |
| October | `9` | 指示十月。 |
| November | `10` | 指示十一月。 |
| December | `11` | 指示十二月。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

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


