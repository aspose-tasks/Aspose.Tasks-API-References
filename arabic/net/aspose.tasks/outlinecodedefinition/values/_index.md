---
title: "OutlineCodeDefinition.Values"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineCodeDefinition. تحصل على كائن OutlineValueCollection. قيم الجدول المرتبط بهذا رمز المخطط"
type: docs
weight: 150
url: /ar/net/aspose.tasks/outlinecodedefinition/values/
---
## OutlineCodeDefinition.Values property

يحصل على كائن OutlineValueCollection. قيم الجدول المرتبط بهذا رمز المخطط.

```csharp
public OutlineValueCollection Values { get; }
```

## الأمثلة

يعرض كيفية إنشاء رموز مخطط جديدة.

```csharp
var project = new Project(DataDir + "project.mpp");

// تعريف رمز المخطط وقناع المخطط الخاص به
var code1 = new OutlineCodeDefinition();
code1.Alias = "New task outline code1";
code1.FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString();
code1.FieldName = "Outline Code1";
var mask = new OutlineMask();
mask.Separator = "+";
mask.Level = 1;
mask.Type = MaskType.Numbers;
code1.Masks.Add(mask);

// إضافة قيمة مخطط
var value = new OutlineValue();
value.Description = "Value description";
value.ValueId = 1;
value.Value = "123456";
value.Type = OutlineValueType.Number;
code1.Values.Add(value);

// إضافة رمز المخطط إلى المشروع
project.OutlineCodes.Add(code1);

// تعريف رمز المخطط وقناع المخطط الخاص به
var code2 = new OutlineCodeDefinition();
code2.Alias = "New rsc outline code2";
code2.FieldId = ((int)ExtendedAttributeResource.OutlineCode2).ToString();
code2.FieldName = "Outline Code2";
var mask2 = new OutlineMask();
mask2.Separator = "/";
mask2.Level = 1;
mask2.Type = MaskType.Numbers;
code2.Masks.Add(mask2);

// إضافة قيمة مخطط
var value2 = new OutlineValue();
value2.Description = "Value2 description";
value2.ValueId = 2;
value2.Value = "987654";
value2.Type = OutlineValueType.Number;
code2.Values.Add(value2);

// إضافة رمز المخطط إلى المشروع
project.OutlineCodes.Add(code2);

project.Save(OutDir + "Updated_project_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [OutlineValueCollection](../../outlinevaluecollection/)
* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


