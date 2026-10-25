---
title: "فئة OutlineValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.OutlineValue. تمثّل قيمة مخطط."
type: docs
weight: 1210
url: /ar/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

يمثل قيمة مخطط تفصيلي.

```csharp
public class OutlineValue
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineValue](outlinevalue/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | يحصل أو يعيّن الوصف لقيمة المخطط. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | يحصل أو يعيّن المدة إذا كان النوع هو Duration. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت قيمة المخطط مطوية أم لا. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | يحصل أو يعيّن المعرف (Id) لعقدة الأب لرمز المخطط. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | يحصل أو يعيّن نوع رمز المخطط. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | يحصل أو يعيّن القيمة الفعلية. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | يحصل على GUID يحدد هذه القيمة بين القيم الأخرى في المشروع بأكمله. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | يحصل أو يعيّن المعرف الفريد (Id) لقيمة رمز المخطط داخل مشروع. |

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


