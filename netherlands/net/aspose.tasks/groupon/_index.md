---
title: "Enum GroupOn"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GroupOn enum. Geeft het type groepering aan"
type: docs
weight: 810
url: /nl/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Specificeert het type groepering.

```csharp
public enum GroupOn
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| DateDay | `13` | Groeperen op datum per dag. |
| DateEachValue | `10` | Groeperen op datum voor elke waarde. |
| DateHour | `12` | Groeperen op datum per uur. |
| DateMinute | `11` | Groeperen op datum per minuut. |
| DateMonth | `16` | Groeperen op datum per maand. |
| DateQtr | `17` | Groeperen op datum per kwartaal. |
| DateThirdOfMonth | `15` | Groeperen op datum per elk derde van een maand. |
| DateWeek | `14` | Groeperen op datum per week. |
| DateYear | `18` | Groeperen op datum per jaar. |
| DurationDays | `23` | Groeperen op duur per dagen. |
| DurationEachValue | `20` | Groeperen op duur voor elke waarde. |
| DurationHours | `22` | Groeperen op duur per uren. |
| DurationMinutes | `21` | Groeperen op duur per minuten. |
| DurationMonths | `25` | Groeperen op duur per maanden. |
| DurationWeeks | `24` | Groeperen op duur per weken. |
| EachValue | `0` | Groeperen per elke waarde. |
| Interval | `1` | Groeperen per het interval. |
| OutlineEachValue | `30` | Groeperen op elke outline-waarde. |
| OutlineLevel | `31` | Groeperen op het outline-niveau. |
| Pct110 | `45` | Groeperen per 10 procent voltooiingsstappen. |
| Pct125 | `44` | Groeperen per 25 procent voltooiingsstappen. |
| Pct150 | `43` | Groeperen per 50 procent voltooiingsstappen. |
| Pct199 | `42` | Groeperen per 99 procent voltooiing. |
| PctEachValue | `40` | Groeperen op procent van elke waarde. |
| PctInterval | `41` | Groeperen op het intervalpercentage. |
| TextEachValue | `50` | Groeperen op elke tekstwaarde. |
| TextPrefix | `51` | Groeperen op het tekstvoorvoegsel. |

## Voorbeelden

Toont hoe de eigenschappen van een groepscriterium gelezen kunnen worden.

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

// lees het achtergrondpatroon van het criterium
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


