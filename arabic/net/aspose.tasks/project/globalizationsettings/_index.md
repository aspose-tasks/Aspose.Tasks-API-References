---
title: "Project.GlobalizationSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية المشروع. تحصل أو تعين إعدادات اللغة الخاصة بالعالمية للمشروع"
type: docs
weight: 460
url: /ar/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

يحصل أو يعيّن إعدادات العولمة (المحددة للغة) للمشروع.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## ملاحظات

الطريقة الموصى بها هي استخدام القيم أو الصيغ غير المتأثرة بالثقافة عبر المشروع. ومع ذلك، إذا كان المشروع يستخدم قيمًا متعلقة بالثقافة، يمكن استخدام هذه الفئة لمساعدة محرك الحساب في تحليل تلك القيم.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


