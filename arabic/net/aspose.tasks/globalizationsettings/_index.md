---
title: "Class GlobalizationSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.GlobalizationSettings class. يمثل إعدادات تعميم المشروع"
type: docs
weight: 720
url: /ar/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

يمثل إعدادات تعميم المشروع.

```csharp
public class GlobalizationSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | يحصل على سلسلة للثابت المنطقي 'false' المستخدم في صيغة. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | يحصل على الثابت "NA" (قيمة فارغة) المستخدم في صيغة لحقل التاريخ. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | يحصل على سلسلة للثابت المنطقي 'true' المستخدم في صيغة. |

## ملاحظات

الطريقة الموصى بها هي استخدام الثوابت أو الصيغ غير المعتمدة على الثقافة عبر المشروع بأكمله. ومع ذلك، إذا كان المشروع يستخدم ثوابت خاصة بالثقافة، يمكن استخدام هذه الفئة لمساعدة محرك حساب الصيغ على تحليل تلك الثوابت.

## الأمثلة

يعرض كيفية ضبط إعدادات اللغة الخاصة بالمشروع.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// إنشاء سمة موسعة
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


