---
title: "GroupCriterion.Ascending"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GroupCriterion. تحصل أو تعيّن قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف مجموعة مُرتّب بترتيب تصاعدي. False إذا كان الحقل مُرتّب بترتيب تنازلي."
type: docs
weight: 20
url: /ar/net/aspose.tasks/groupcriterion/ascending/
---
## GroupCriterion.Ascending property

يحصل أو يضبط قيمة تشير إلى ما إذا كان الحقل المستخدم كمعيار في تعريف مجموعة يتم فرزه بترتيب تصاعدي. خطأ إذا تم فرز الحقل بترتيب تنازلي.

```csharp
public bool Ascending { get; set; }
```

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

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


