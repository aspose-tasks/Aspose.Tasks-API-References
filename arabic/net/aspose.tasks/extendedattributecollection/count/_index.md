---
title: "ExtendedAttributeCollection.Count"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttributeCollection. تحصل على عدد العناصر الموجودة في هذه المجموعة"
type: docs
weight: 10
url: /ar/net/aspose.tasks/extendedattributecollection/count/
---
## ExtendedAttributeCollection.Count property

يحصل على عدد العناصر الموجودة في هذه المجموعة.

```csharp
public int Count { get; }
```

## الأمثلة

يعرض كيفية استخدام مجموعات السمات الموسعة.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// احصل على مهمة الفهرس صفر
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // مسح السمات الموسعة
    task.ExtendedAttributes.Clear();
}

// إنشاء تعريف سمة موسعة لمهمة
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// إضافة سمة موسعة 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// إضافة سمة موسعة 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// العمل مع السمات الموسعة...

// إزالة سمة موسعة حسب الفهرس
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// استخدام وصول الفهرس للمجموعة
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// نسخ السمات إلى مشروع آخر
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// إزالة جميع تعريفات السمات الموسعة
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### انظر أيضًا

* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


