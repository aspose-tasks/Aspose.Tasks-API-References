---
title: "OutlineMaskCollection.IsReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineMaskCollection. تحصل على قيمة تشير إلى ما إذا كان هذا التجميع للقراءة فقط أم لا"
type: docs
weight: 20
url: /ar/net/aspose.tasks/outlinemaskcollection/isreadonly/
---
## OutlineMaskCollection.IsReadOnly property

يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

```csharp
public bool IsReadOnly { get; }
```

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

* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


