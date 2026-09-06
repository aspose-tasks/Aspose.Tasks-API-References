---
title: "تعداد GroupOn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.GroupOn enum. يحدد نوع التجميع"
type: docs
weight: 810
url: /ar/net/aspose.tasks/groupon/
---
## GroupOn enumeration

يحدد نوع التجميع.

```csharp
public enum GroupOn
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DateDay | `13` | تجميع حسب التاريخ يوميًا. |
| DateEachValue | `10` | تجميع حسب التاريخ لكل قيمة. |
| DateHour | `12` | تجميع حسب التاريخ بالساعة. |
| DateMinute | `11` | تجميع حسب التاريخ بالدقيقة. |
| DateMonth | `16` | تجميع حسب التاريخ بالشهر. |
| DateQtr | `17` | تجميع حسب التاريخ بالربع. |
| DateThirdOfMonth | `15` | تجميع حسب التاريخ بكل ثالث من الشهر. |
| DateWeek | `14` | تجميع حسب التاريخ بالأسبوع. |
| DateYear | `18` | تجميع حسب التاريخ بالسنة. |
| DurationDays | `23` | تجميع حسب المدة بالأيام. |
| DurationEachValue | `20` | تجميع حسب المدة لكل قيمة. |
| DurationHours | `22` | تجميع حسب المدة بالساعات. |
| DurationMinutes | `21` | تجميع حسب المدة بالدقائق. |
| DurationMonths | `25` | تجميع حسب المدة بالأشهر. |
| DurationWeeks | `24` | تجميع حسب المدة بالأسابيع. |
| EachValue | `0` | تجميع حسب كل قيمة. |
| Interval | `1` | تجميع حسب الفاصل الزمني. |
| OutlineEachValue | `30` | تجميع لكل قيمة مخطط. |
| OutlineLevel | `31` | تجميع على مستوى المخطط. |
| Pct110 | `45` | تجميع بزيادات إكمال بنسبة 10٪. |
| Pct125 | `44` | تجميع بزيادات إكمال بنسبة 25٪. |
| Pct150 | `43` | تجميع بزيادات إكمال بنسبة 50٪. |
| Pct199 | `42` | تجميع بنسبة إكمال 99٪. |
| PctEachValue | `40` | تجميع على نسبة كل قيمة. |
| PctInterval | `41` | تجميع على نسبة الفاصل الزمني. |
| TextEachValue | `50` | تجميع على كل قيمة نصية. |
| TextPrefix | `51` | تجميع على بادئة النص. |

## الأمثلة

يعرض كيفية قراءة خصائص معيار المجموعة.

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

// قراءة نمط الخلفية للمعيار
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


