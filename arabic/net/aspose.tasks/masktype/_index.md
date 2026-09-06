---
title: "تعداد MaskType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.MaskType تعداد. يحدد نوع القناع"
type: docs
weight: 1000
url: /ar/net/aspose.tasks/masktype/
---
## MaskType enumeration

يحدد نوع القناع.

```csharp
public enum MaskType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Null | `0` | يشير إلى نوع القناع Null. |
| Numbers | `1` | يشير إلى نوع القناع Numbers. |
| UpperCaseLetters | `2` | يشير إلى نوع القناع UpperCaseLetters. |
| LowerCaseLetters | `3` | يشير إلى نوع القناع LowerCaseLetters. |
| Characters | `4` | يشير إلى نوع القناع Characters. |
| Val4 | `5` | يشير إلى نوع القناع Lookup for Cost. |
| Val5 | `6` | يشير إلى نوع القناع Lookup for Dates. |
| Val6 | `7` | يشير إلى نوع القناع Lookup for Durations. |
| Val7 | `8` | يشير إلى نوع القناع Lookup for Numbers. |
| Val8 | `9` | يشير إلى نوع القناع Lookup for Flags. |
| Val9 | `10` | يشير إلى نوع القناع Lookup for FinishDate. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


