---
title: "التعداد OutlineValueType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.OutlineValueType. يحدد نوع قيمة المخطط"
type: docs
weight: 1230
url: /ar/net/aspose.tasks/outlinevaluetype/
---
## OutlineValueType enumeration

يحدد نوع قيمة المخطط.

```csharp
public enum OutlineValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Null | `0` | يشير إلى نوع قيمة المخطط Null. |
| Date | `1` | يشير إلى نوع قيمة المخطط Date. |
| Duration | `2` | يشير إلى نوع قيمة المخطط Duration. |
| Cost | `3` | يشير إلى نوع قيمة المخطط Cost. |
| Number | `4` | يشير إلى نوع قيمة المخطط Number. |
| Flag | `5` | يشير إلى نوع قيمة المخطط للعلامة. |
| Text | `6` | يشير إلى نوع قيمة المخطط للنص. |
| FinishDate | `7` | يشير إلى نوع قيمة المخطط لتاريخ الانتهاء. |

## الأمثلة

يوضح كيفية العمل مع قيم المخطط.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// إنشاء قيمة مخطط
var value = new OutlineValue();

// تعيين القيمة الفعلية
value.Value = "Text value 1";

// تعيين المعرف الفريد لقيمة رمز المخطط داخل المشروع
value.ValueId = 1;

// الحصول على GUID يحدد هذه القيمة بين القيم الأخرى في المشروع بأكمله
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// تعيين نوع رمز المخطط
value.Type = OutlineValueType.Text;

// تعيين وصف قيمة المخطط
value.Description = "Text value descr 1";

// تعيين قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا
value.IsCollapsed = false;

// التحقق من معرف القيمة الأصلية
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// إنشاء قيمة مخطط مع المدة
var value2 = new OutlineValue();

// تعيين قيمة المدة
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// تعيين المعرف الفريد لقيمة رمز المخطط داخل المشروع
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


