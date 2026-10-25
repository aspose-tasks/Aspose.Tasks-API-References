---
title: "OutlineCodeDefinition.Enterprise"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineCodeDefinition. يحصل أو يعيّن قيمة تشير إلى ما إذا كان رمز المخطط المخصص هو رمز مخطط مخصص للمؤسسة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/outlinecodedefinition/enterprise/
---
## OutlineCodeDefinition.Enterprise property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان رمز المخطط المخصص هو رمز مخطط مخصص للمؤسسة.

```csharp
public bool Enterprise { get; set; }
```

## الأمثلة

يعرض كيفية العمل مع تعريفات رموز المخطط.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// إنشاء تعريف جديد لرمز المخطط
var outline = new OutlineCodeDefinition();

// تعيين رقم الحقل لرمز المخطط
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// تعيين اسم رمز مخطط مخصص
outline.FieldName = "Outline Code1";

// تعيين الـ Guid لرمز المخطط
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// تعيين قيمة تشير إلى ما إذا كانت القيم المحددة في حقل رمز المخطط هذا يجب أن تكون قيمًا نهائية
outline.LeafOnly = false;

// تعيين الاسم المستعار لرمز مخطط مخصص
outline.Alias = "My Outline Code";

// تعيين النطق الصوتي للاسم المستعار لرمز المخطط المخصص
outline.PhoneticAlias = "Outline Code";

// تعيين قيمة تشير إلى ما إذا كان يجب أن تحتوي الرموز الجديدة على جميع المستويات. غير متاح لرموز المؤسسة.
outline.AllLevelsRequired = true;

// تعيين قيمة تشير إلى ما إذا كان رمز المخطط المخصص هو رمز مخطط مخصص للمؤسسة
outline.Enterprise = false;

// تعيين إشارة إلى حقل مخصص آخر يكون هذا التعريف لرمز المخطط بمثابة اسم مستعار له
outline.EnterpriseOutlineCodeAlias = 0;

// إضافة قناع مخطط
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// تعيين قيمة تشير إلى ما إذا كان يجب أن تأتي القيم المحددة من جدول القيم
outline.OnlyTableValuesAllowed = false;

// تعيين قيمة تشير إلى ما إذا كان يمكن استخدام رمز المخطط المخصص
// عن طريق معالج استبدال الموارد في Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// تعيين قيمة تشير إلى ما إذا كان يجب إظهار مسافات الإدخال لهذا رمز المخطط.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### انظر أيضًا

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


