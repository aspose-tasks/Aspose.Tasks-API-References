---
title: "الفئة ExtendedAttribute"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.ExtendedAttribute. تمثل السمات الموسعة"
type: docs
weight: 520
url: /ar/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

يمثل السمات الموسعة.

```csharp
public class ExtendedAttribute
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | يحصل على تعريف السمة. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | يحصل أو يعيّن قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | يحصل أو يعيّن قيمة للسمات ذات النوع 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | يحصل على معرّف الحقل. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان العلم مُعيّنًا للصفة ذات النوع 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | يحصل على ما إذا كان حساب قيمة السمة الموسعة قد نتج عنه خطأ. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | يحصل أو يعيّن قيمة للسمات ذات الأنواع الرقمية (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | يحصل أو يعيّن قيمة للسمات ذات النوع 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | يحصل على الـ guid لقيمة البحث. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت قيمة هذا الكائن `ExtendedAttribute` للقراءة فقط. تُرجع true إذا تم تعريف صيغة أو تجميع في [`ExtendedAttributeDefinition`](../extendedattributedefinition/) لهذا الكائن. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | يعيد تمثيل نصي قصير للسمة الموسعة. |

## ملاحظات

حاليًا يتم دعم جميع أنواع السمات الموسعة عند القراءة من MSP Xml 2003/2007 و mpp 2003. بالنسبة إلى MSP mpp 2007 يتم دعم قراءة جميع السمات الموسعة باستثناء الفترات الزمنية والعلامات.

## الأمثلة

يوضح كيفية إضافة حقل مخصص يتم حساب قيمته باستخدام صيغة يحددها المستخدم.

```csharp
var project = new Project();

// إنشاء تعريف سمة موسعة جديدة للمهمة
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// أضف صيغة إلى السمة.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// إنشاء سمة موسعة
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// نقوم بتعيين الصيغة للسمة الموسعة، لذا فهي للقراءة فقط (يتم حساب القيمة باستخدام الصيغة).
// الناتج هو "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// يمكنك محاولة تعيين قيمة لحقل للقراءة فقط، لكن ذلك لن يكون له أي تأثير.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


