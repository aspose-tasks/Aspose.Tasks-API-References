---
title: "الفئة SplitPartCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.SplitPartCollection. مجموعة تمثل أجزاء مهمة."
type: docs
weight: 2300
url: /ar/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

مجموعة تمثل أجزاء المهمة.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | يحصل على عدد الأجزاء في المجموعة. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | يسترجع الجزء المقسّم للمهمة عند الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | ينسخ جميع الأجزاء من المجموعة إلى مصفوفة جديدة. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


