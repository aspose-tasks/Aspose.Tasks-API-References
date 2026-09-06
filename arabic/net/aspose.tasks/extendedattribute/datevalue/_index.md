---
title: "ExtendedAttribute.DateValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. تحصل أو تعين قيمة للسمات ذات أنواع التاريخ Date Start Finish."
type: docs
weight: 20
url: /ar/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

يحصل أو يعيّن قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish).

```csharp
public DateTime DateValue { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يُرمى إذا لم يتم تهيئة خاصية [`AttributeDefinition`](../attributedefinition/) أو إذا لم تكن السمة الحالية سمة تاريخ. |

## الأمثلة

يعرض كيفية تغيير تعريف السمة للخاصية الموسعة.

```csharp
var project = new Project();

// إنشاء تعريف سمة موسعة جديدة للمهمة
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// أضف صيغة إلى الخاصية.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// إنشاء خاصية موسعة
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// إنشاء تعريف سمة موسعة جديدة من نوع التاريخ
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// أضف صيغة إلى الخاصية.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### انظر أيضًا

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


