---
title: "SplitPartCollection.GetEnumerator"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة SplitPartCollection. تُرجع مُعدِّدًا لهذه المجموعة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

يرجع عدادًا لهذه المجموعة.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### قيمة الإرجاع

عداد لهذه المجموعة.

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


