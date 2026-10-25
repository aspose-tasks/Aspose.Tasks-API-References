---
title: "OutlineMaskCollection.Contains"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة OutlineMaskCollection. تُرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة وإلا false"
type: docs
weight: 60
url: /ar/net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.

```csharp
public bool Contains(OutlineMask item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | OutlineMask | العنصر المحدد للبحث عنه. |

### قيمة الإرجاع

صحيح إذا وُجد العنصر المحدد في هذه المجموعة؛ وإلا، خطأ.

## الأمثلة

يعرض كيفية العمل مع مجموعات أقنعة المخطط التفصيلي.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// مسح أقنعة المخطط
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// إدراج قناع غير صحيح
outline.Masks.Insert(0, maskWrong);

// تحرير القناع باستخدام وصول الفهرس للمجموعة
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// إزالة قناع غير صحيح باستخدام الفهرس
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// التكرار عبر الأقنعة
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### انظر أيضًا

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


