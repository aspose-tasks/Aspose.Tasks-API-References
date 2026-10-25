---
title: "ExtendedAttribute.AttributeDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. يحصل على تعريف السمة"
type: docs
weight: 10
url: /ar/net/aspose.tasks/extendedattribute/attributedefinition/
---
## ExtendedAttribute.AttributeDefinition property

يحصل على تعريف السمة.

```csharp
public ExtendedAttributeDefinition AttributeDefinition { get; }
```

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

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


