---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. تزيل قيمة من قائمة البحث الداخلية. هذه طريقة مفضلة للتعامل مع ValueList"
type: docs
weight: 340
url: /ar/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

يزيل قيمة من قائمة البحث الداخلية. هذه طريقة مفضلة للتعامل مع [`ValueList`](../valuelist/).

```csharp
public void RemoveLookupValue(Value value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| value | القيمة | القيمة لإزالتها من البحث. |

## ملاحظات

هذه الطريقة تعمل فقط مع حالات [`ExtendedAttributeDefinition`](../) التي يكون فيها [`CalculationType`](../calculationtype/) مساويًا لـ Lookup.

## الأمثلة

يظهر كيفية إضافة سمات موسعة مع قوائم اختيار للتعيينات.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// تعيين المورد "1 TRG: Trade Group" إلى "TASK 1" بإنشاء كائن ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// إنشاء تعريف سمة مخصصة مع قائمة اختيار.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// يمكن رؤية هذه القيمة في عرض "Resource usage" في MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// إنشاء تعريف سمة مخصصة مع قائمة اختيار.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// يمكن رؤية هذه القيمة في عرض "Task usage" في MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// يمكن إزالة القيم الخاطئة لاحقًا.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// العمل مع المشروع...
```

### انظر أيضًا

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


