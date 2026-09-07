---
title: "एनम GroupOn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GroupOn enum. समूह बनाने के प्रकार को निर्दिष्ट करता है"
type: docs
weight: 810
url: /hi/net/aspose.tasks/groupon/
---
## GroupOn enumeration

समूह बनाने के प्रकार को निर्दिष्ट करता है।

```csharp
public enum GroupOn
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| DateDay | `13` | तिथि को दिन के अनुसार समूहित करें। |
| DateEachValue | `10` | प्रत्येक मान के लिए तिथि को समूहित करें। |
| DateHour | `12` | घंटे के आधार पर तिथि को समूहित करें। |
| DateMinute | `11` | मिनट के आधार पर तिथि को समूहित करें। |
| DateMonth | `16` | महीने के आधार पर तिथि को समूहित करें। |
| DateQtr | `17` | त्रैमासिक के आधार पर तिथि को समूहित करें। |
| DateThirdOfMonth | `15` | महीने के प्रत्येक तिहाई के आधार पर तिथि को समूहित करें। |
| DateWeek | `14` | सप्ताह के आधार पर तिथि को समूहित करें। |
| DateYear | `18` | वर्ष के आधार पर तिथि को समूहित करें। |
| DurationDays | `23` | दिनों के आधार पर अवधि को समूहित करें। |
| DurationEachValue | `20` | प्रत्येक मान के लिए अवधि को समूहित करें। |
| DurationHours | `22` | घंटों के आधार पर अवधि को समूहित करें। |
| DurationMinutes | `21` | मिनटों के आधार पर अवधि को समूहित करें। |
| DurationMonths | `25` | महीनों के आधार पर अवधि को समूहित करें। |
| DurationWeeks | `24` | सप्ताहों के आधार पर अवधि को समूहित करें। |
| EachValue | `0` | प्रत्येक मान के अनुसार समूहित करें। |
| Interval | `1` | अंतराल के अनुसार समूहित करें। |
| OutlineEachValue | `30` | प्रत्येक रूपरेखा मान के अनुसार समूहित करें। |
| OutlineLevel | `31` | रूपरेखा स्तर के अनुसार समूहित करें। |
| Pct110 | `45` | 10 प्रतिशत पूर्णता वृद्धि के अनुसार समूहित करें। |
| Pct125 | `44` | 25 प्रतिशत पूर्णता वृद्धि के अनुसार समूहित करें। |
| Pct150 | `43` | 50 प्रतिशत पूर्णता वृद्धि के अनुसार समूहित करें। |
| Pct199 | `42` | 99 प्रतिशत पूर्णता के अनुसार समूहित करें। |
| PctEachValue | `40` | प्रत्येक मान के प्रतिशत के अनुसार समूहित करें। |
| PctInterval | `41` | अंतराल प्रतिशत के अनुसार समूहित करें। |
| TextEachValue | `50` | प्रत्येक पाठ मान के अनुसार समूहित करें। |
| TextPrefix | `51` | पाठ उपसर्ग के अनुसार समूहित करें। |

## उदाहरण

दिखाता है कि समूह मानदंड की गुणों को कैसे पढ़ें।

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

// मानदंड की पृष्ठभूमि पैटर्न पढ़ें।
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


