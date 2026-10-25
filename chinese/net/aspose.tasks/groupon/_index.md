---
title: "枚举 GroupOn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GroupOn 枚举。指定分组的类型"
type: docs
weight: 810
url: /zh/net/aspose.tasks/groupon/
---
## GroupOn enumeration

指定分组的类型。

```csharp
public enum GroupOn
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DateDay | `13` | 按天对日期进行分组。 |
| DateEachValue | `10` | 对每个值的日期进行分组。 |
| DateHour | `12` | 按小时对日期进行分组。 |
| DateMinute | `11` | 按分钟对日期进行分组。 |
| DateMonth | `16` | 按月份对日期进行分组。 |
| DateQtr | `17` | 按季度对日期进行分组。 |
| DateThirdOfMonth | `15` | 按每月的三分之一对日期进行分组。 |
| DateWeek | `14` | 按周对日期进行分组。 |
| DateYear | `18` | 按年份对日期进行分组。 |
| DurationDays | `23` | 按天对持续时间进行分组。 |
| DurationEachValue | `20` | 对每个值的持续时间进行分组。 |
| DurationHours | `22` | 按小时对持续时间进行分组。 |
| DurationMinutes | `21` | 按分钟对持续时间进行分组。 |
| DurationMonths | `25` | 按月份对持续时间进行分组。 |
| DurationWeeks | `24` | 按周对持续时间进行分组。 |
| EachValue | `0` | 按每个值进行分组。 |
| Interval | `1` | 按间隔进行分组。 |
| OutlineEachValue | `30` | 对每个大纲值进行分组。 |
| OutlineLevel | `31` | 对大纲级别进行分组。 |
| Pct110 | `45` | 按10%完成增量进行分组。 |
| Pct125 | `44` | 按25%完成增量进行分组。 |
| Pct150 | `43` | 按50%完成增量进行分组。 |
| Pct199 | `42` | 按99%完成进行分组。 |
| PctEachValue | `40` | 对每个值的百分比进行分组。 |
| PctInterval | `41` | 对间隔百分比进行分组。 |
| TextEachValue | `50` | 对每个文本值进行分组。 |
| TextPrefix | `51` | 对文本前缀进行分组。 |

## 示例

展示如何读取组准则的属性。

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// 读取准则的背景模式。
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


