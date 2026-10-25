---
title: "Перечисление GroupOn"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.GroupOn. Указывает тип группировки"
type: docs
weight: 810
url: /ru/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Указывает тип группировки.

```csharp
public enum GroupOn
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| DateDay | `13` | Группировать по дате по дням. |
| DateEachValue | `10` | Группировать по дате для каждого значения. |
| DateHour | `12` | Группировать по дате по часам. |
| DateMinute | `11` | Группировать по дате по минутам. |
| DateMonth | `16` | Группировать по дате по месяцам. |
| DateQtr | `17` | Группировать по дате по кварталам. |
| DateThirdOfMonth | `15` | Группировать по дате по каждой трети месяца. |
| DateWeek | `14` | Группировать по дате по неделям. |
| DateYear | `18` | Группировать по дате по годам. |
| DurationDays | `23` | Группировать по длительности по дням. |
| DurationEachValue | `20` | Группировать по длительности для каждого значения. |
| DurationHours | `22` | Группировать по длительности по часам. |
| DurationMinutes | `21` | Группировать по длительности по минутам. |
| DurationMonths | `25` | Группировать по длительности по месяцам. |
| DurationWeeks | `24` | Группировать по длительности по неделям. |
| EachValue | `0` | Группировать по каждому значению. |
| Interval | `1` | Группировать по интервалу. |
| OutlineEachValue | `30` | Группировать по каждому значению контура. |
| OutlineLevel | `31` | Группировать по уровню контура. |
| Pct110 | `45` | Группировать по приросту завершения 10 процентов. |
| Pct125 | `44` | Группировать по приросту завершения 25 процентов. |
| Pct150 | `43` | Группировать по приросту завершения 50 процентов. |
| Pct199 | `42` | Группировать по завершению 99 процентов. |
| PctEachValue | `40` | Группировать по проценту каждого значения. |
| PctInterval | `41` | Группировать по проценту интервала. |
| TextEachValue | `50` | Группировать по каждому текстовому значению. |
| TextPrefix | `51` | Группировать по префиксу текста. |

## Примеры

Показывает, как читать свойства группового критерия.

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

// читать фоновый шаблон критерия  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


