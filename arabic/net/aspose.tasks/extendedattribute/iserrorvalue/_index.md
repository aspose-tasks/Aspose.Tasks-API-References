---
title: "ExtendedAttribute.IsErrorValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. يحصل على ما إذا كان حساب قيمة السمات الموسعة نتج عنه خطأ"
type: docs
weight: 60
url: /ar/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

يحصل على ما إذا كان حساب قيمة السمة الموسعة قد نتج عنه خطأ.

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


