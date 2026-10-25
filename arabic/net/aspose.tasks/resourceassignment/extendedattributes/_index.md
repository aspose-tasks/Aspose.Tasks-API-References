---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ResourceAssignment. تحصل أو تعين نسخة من فئة ExtendedAttributeCollection لهذا الكائن"
type: docs
weight: 250
url: /ar/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

يحصل أو يعيّن نسخة من الفئة ExtendedAttributeCollection لهذا الكائن.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## ملاحظات

القراءة مدعومة لتنسيق XML فقط.

## الأمثلة

يوضح كيفية إضافة سمات موسعة لتعيين.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// تعيين المورد "1 TRG: Trade Group" إلى "TASK 1" بإنشاء كائن ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// إنشاء تعريف سمة مخصصة مع قائمة اختيار.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// يمكن رؤية هذه القيمة في عرض "Resource usage" في MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### انظر أيضًا

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


