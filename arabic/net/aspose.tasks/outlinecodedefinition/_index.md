---
title: "الفئة OutlineCodeDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OutlineCodeDefinition. تمثل تعريف رمز المخطط."
type: docs
weight: 1170
url: /ar/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

يمثل تعريفًا لرمز المخطط التفصيلي.

```csharp
public sealed class OutlineCodeDefinition
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | ينشئ مثيلًا جديدًا للفئة `OutlineCodeDefinition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | يحصل أو يعيّن الاسم المستعار لرمز مخطط مخصص. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب أن تحتوي الرموز الجديدة على جميع المستويات. غير متوفر لرموز المؤسسة. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان رمز المخطط المخصص هو رمز مخطط مخصص للمؤسسة. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | يحصل أو يعيّن إشارة إلى حقل مخصص آخر يكون هذا التعريف لرمز المخطط هو الاسم المستعار له. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | يحصل أو يعيّن رقم الحقل لرمز المخطط. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | يحصل أو يعيّن اسم رمز المخطط المخصص. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | يحصل أو يعيّن المعرف الفريد (Guid) لرمز المخطط. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب أن تكون القيم المحددة في حقل رمز المخطط هذا قيمًا نهائية. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | يحصل على كائن OutlineMaskCollection. جدول الإدخالات الذي يحدد قناع رمز المخطط. نسخة للقراءة فقط من [`OutlineMaskCollection`](../outlinemaskcollection/). |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب أن تأتي القيم المحددة من جدول القيم. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | يحصل أو يعيّن النطق الفونيمي للاسم المستعار لرمز المخطط المخصص. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يمكن استخدام رمز المخطط المخصص بواسطة معالج استبدال الموارد في Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إظهار المسافات البادئة لهذا رمز المخطط. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | يحصل على كائن OutlineValueCollection. قيم الجدول المرتبط بهذا رمز المخطط. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


