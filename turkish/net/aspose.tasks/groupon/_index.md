---
title: "Enum GroupOn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GroupOn enum. Gruplandırma türünü belirtir"
type: docs
weight: 810
url: /tr/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Gruplamanın türünü belirtir.

```csharp
public enum GroupOn
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DateDay | `13` | Tarihe göre günü grupla. |
| DateEachValue | `10` | Tarihe göre her değer için grupla. |
| DateHour | `12` | Tarihi saate göre grupla. |
| DateMinute | `11` | Tarihi dakikaya göre grupla. |
| DateMonth | `16` | Tarihi aya göre grupla. |
| DateQtr | `17` | Tarihi çeyreğe göre grupla. |
| DateThirdOfMonth | `15` | Tarihi ayın her üçte birine göre grupla. |
| DateWeek | `14` | Tarihi haftaya göre grupla. |
| DateYear | `18` | Tarihi yıla göre grupla. |
| DurationDays | `23` | Süreyi günlere göre grupla. |
| DurationEachValue | `20` | Süreyi her değer için grupla. |
| DurationHours | `22` | Süreyi saatlere göre grupla. |
| DurationMinutes | `21` | Süreyi dakikalara göre grupla. |
| DurationMonths | `25` | Süreyi aylara göre grupla. |
| DurationWeeks | `24` | Süreyi haftalara göre grupla. |
| EachValue | `0` | Her değere göre grupla. |
| Interval | `1` | Aralığa göre grupla. |
| OutlineEachValue | `30` | Her anahat değerine göre grupla. |
| OutlineLevel | `31` | Anahat seviyesine göre grupla. |
| Pct110 | `45` | %10 tamamlama artışına göre grupla. |
| Pct125 | `44` | %25 tamamlama artışına göre grupla. |
| Pct150 | `43` | %50 tamamlama artışına göre grupla. |
| Pct199 | `42` | %99 tamamlama oranına göre grupla. |
| PctEachValue | `40` | Her değerin yüzdesine göre grupla. |
| PctInterval | `41` | Aralık yüzdesine göre grupla. |
| TextEachValue | `50` | Her metin değerine göre grupla. |
| TextPrefix | `51` | Metin önekine göre grupla. |

## Örnekler

Bir grup kriterinin özelliklerini nasıl okuyacağınızı gösterir.

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

// Kriterin arka plan desenini okuyun.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


