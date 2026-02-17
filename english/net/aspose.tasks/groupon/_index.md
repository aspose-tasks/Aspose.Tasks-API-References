---
title: Enum GroupOn
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GroupOn enum. Specifies the type of grouping
type: docs
weight: 810
url: /net/aspose.tasks/groupon/
---
## GroupOn enumeration

Specifies the type of grouping.

```csharp
public enum GroupOn
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| DateDay | `13` | Group on date by day. |
| DateEachValue | `10` | Group on date for each value. |
| DateHour | `12` | Group on date by hour. |
| DateMinute | `11` | Group on date by minute. |
| DateMonth | `16` | Group on date by month. |
| DateQtr | `17` | Group on date by quarter. |
| DateThirdOfMonth | `15` | Group on date by each third of a month. |
| DateWeek | `14` | Group on date by week. |
| DateYear | `18` | Group on date by year. |
| DurationDays | `23` | Group on duration by days. |
| DurationEachValue | `20` | Group on duration for each value. |
| DurationHours | `22` | Group on duration by hours. |
| DurationMinutes | `21` | Group on duration by minutes. |
| DurationMonths | `25` | Group on duration by months. |
| DurationWeeks | `24` | Group on duration by weeks. |
| EachValue | `0` | Group by each value. |
| Interval | `1` | Group by the interval. |
| OutlineEachValue | `30` | Group on each outline value. |
| OutlineLevel | `31` | Group on the outline level. |
| Pct110 | `45` | Group by 10 percent completion increments. |
| Pct125 | `44` | Group by 25 percent completion increments. |
| Pct150 | `43` | Group by 50 percent completion increments. |
| Pct199 | `42` | Group by 99 percent completion. |
| PctEachValue | `40` | Group on percent of each value. |
| PctInterval | `41` | Group on the interval percent. |
| TextEachValue | `50` | Group on each text value. |
| TextPrefix | `51` | Group on the text prefix. |

## Examples

Shows how to read properties of a group criterion.

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

// read the background pattern of the criterion  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


