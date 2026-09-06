---
title: "SplitPartCollection.Item"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SplitPartCollection. تسترجع جزء تقسيم المهمة عند الفهرس المحدد"
type: docs
weight: 20
url: /ar/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

يسترجع الجزء المقسّم للمهمة عند الفهرس المحدد.

```csharp
public SplitPart this[int index] { get; set; }
```

| معامل | الوصف |
| --- | --- |
| الفهرس | فهرس الجزء. |

### قيمة الإرجاع

جزء مقسّم.

## ملاحظات

الفهرس يبدأ من الصفر. تُعيد null إذا كان الفهرس خارج حدود المصفوفة.

## الأمثلة

يظهر كيفية العمل مع مجموعات الأجزاء المقسمة.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// التكرار على الأجزاء المقسمة
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// احصل على الجزء حسب الفهرس
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// قم ببعض العمل مع الجزء المقسّم الأول للمهمة
```

### انظر أيضًا

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


