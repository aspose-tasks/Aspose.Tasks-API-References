---
title: "ExtendedAttributeDefinition.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinition. تُرجع علامة تُشير إلى ما إذا كانت هذه المثيلة مساوية للكائن المحدد."
type: docs
weight: 320
url: /ar/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

يرجع علامة تشير إلى ما إذا كانت هذه المثيلة مساوية للعنصر المحدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن المحدد للمقارنة بهذه المثيلة. |

### قيمة الإرجاع

علامة تُشير إلى ما إذا كانت هذه المثيلة مساوية للكائن المحدد.

## الأمثلة

يُظهر كيفية التحقق من مساواة تعريف السمة الموسعة.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// يتم التحقق من مساواة التقويمات مقابل معرفات حقول تعريف السمة.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### انظر أيضًا

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


