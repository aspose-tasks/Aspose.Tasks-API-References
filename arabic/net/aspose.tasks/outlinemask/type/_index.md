---
title: "OutlineMask.Type"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineMask. تحصل أو تعيين نوع القناع."
type: docs
weight: 50
url: /ar/net/aspose.tasks/outlinemask/type/
---
## OutlineMask.Type property

يحصل أو يضبط نوع القناع.

```csharp
public MaskType Type { get; set; }
```

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

* enum [MaskType](../../masktype/)
* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


