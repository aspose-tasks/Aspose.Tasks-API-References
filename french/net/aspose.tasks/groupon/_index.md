---
title: "Enum GroupOn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.GroupOn enum. Spécifie le type de regroupement"
type: docs
weight: 810
url: /fr/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Spécifie le type de regroupement.

```csharp
public enum GroupOn
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DateDay | `13` | Regrouper par date par jour. |
| DateEachValue | `10` | Regrouper par date pour chaque valeur. |
| DateHour | `12` | Regrouper par date par heure. |
| DateMinute | `11` | Regrouper par date par minute. |
| DateMonth | `16` | Regrouper par date par mois. |
| DateQtr | `17` | Regrouper par date par trimestre. |
| DateThirdOfMonth | `15` | Regrouper par date par chaque tiers du mois. |
| DateWeek | `14` | Regrouper par date par semaine. |
| DateYear | `18` | Regrouper par date par an. |
| DurationDays | `23` | Regrouper par durée par jours. |
| DurationEachValue | `20` | Regrouper par durée pour chaque valeur. |
| DurationHours | `22` | Regrouper par durée par heures. |
| DurationMinutes | `21` | Regrouper par durée par minutes. |
| DurationMonths | `25` | Regrouper par durée par mois. |
| DurationWeeks | `24` | Regrouper par durée par semaines. |
| EachValue | `0` | Regrouper par chaque valeur. |
| Interval | `1` | Regrouper par l'intervalle. |
| OutlineEachValue | `30` | Regrouper par chaque valeur de contour. |
| OutlineLevel | `31` | Regrouper par le niveau de contour. |
| Pct110 | `45` | Regrouper par incréments de progression de 10 %. |
| Pct125 | `44` | Regrouper par incréments de progression de 25 %. |
| Pct150 | `43` | Regrouper par incréments de progression de 50 %. |
| Pct199 | `42` | Regrouper par progression de 99 %. |
| PctEachValue | `40` | Regrouper par pourcentage de chaque valeur. |
| PctInterval | `41` | Regrouper par le pourcentage d'intervalle. |
| TextEachValue | `50` | Regrouper par chaque valeur de texte. |
| TextPrefix | `51` | Regrouper par le préfixe de texte. |

## Exemples

Montre comment lire les propriétés d'un critère de groupe.

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

// lire le motif de fond du critère  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


