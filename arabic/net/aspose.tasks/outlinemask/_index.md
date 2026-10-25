---
title: "الفئة OutlineMask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OutlineMask. تمثل أربعة عناصر من القناع الذي يحدد تنسيق رمز المخطط"
type: docs
weight: 1190
url: /ar/net/aspose.tasks/outlinemask/
---
## OutlineMask class

يمثل أربعة عناصر من قناع يحدد تنسيق رمز المخطط التفصيلي.

```csharp
public class OutlineMask
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineMask](outlinemask/)() | ينشئ مثيلاً جديدًا للفئة `OutlineMask`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | يحصل أو يعيّن الحد الأقصى للطول (بالحروف) لقيم رمز المخطط. 0 إذا لم يتم تعريف الطول. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | يحصل أو يعيّن مستوى القناع. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | يحصل أو يضبط الفاصل لقيم الشيفرة. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | يحصل أو يضبط نوع القناع. |

## الأمثلة

يعرض كيفية العمل مع أقنعة المخطط التفصيلي.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// اضبط نوع القناع
mask.Type = MaskType.Characters;

// اضبط الفاصل لقيم الشيفرة
mask.Separator = "/";

// اضبط مستوى القناع
mask.Level = 1;

// اضبط الحد الأقصى للطول (بالحروف) لقيم الشيفرة التفصيلية. 0 إذا لم يتم تعريف الطول.
mask.Length = 2;

// أضف القناع إلى التعريف
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


