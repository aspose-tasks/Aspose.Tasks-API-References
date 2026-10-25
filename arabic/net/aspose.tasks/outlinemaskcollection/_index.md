---
title: "الفئة OutlineMaskCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.OutlineMaskCollection. تمثل مجموعة من كائنات OutlineMask"
type: docs
weight: 1200
url: /ar/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

تمثل مجموعة من كائنات [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


