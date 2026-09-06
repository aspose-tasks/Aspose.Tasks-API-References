---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. تُرجع قيمة تجزئة (hash code) للمثيلة من فئة ExtendedAttributeDefinition."
type: docs
weight: 330
url: /ar/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

تُرجع قيمة تجزئة للمثيلة من فئة [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

قيمة تجزئة لهذا الكائن.

## الأمثلة

يُظهر كيفية الحصول على قيمة تجزئة لتعريف سمة موسعة.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// قيمة التجزئة لتعريف سمة موسعة تساوي معرف حقل.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### انظر أيضًا

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


