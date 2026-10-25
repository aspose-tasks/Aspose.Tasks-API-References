---
title: "ExtendedAttribute.ToString"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttribute. تُرجع تمثيلًا نصيًا مختصرًا لخاصية موسعة."
type: docs
weight: 110
url: /ar/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

يعيد تمثيل نصي قصير للسمة الموسعة.

```csharp
public override string ToString()
```

### قيمة الإرجاع

التمثيل النصي للخاصية الموسعة.

## الأمثلة

يوضح كيفية قراءة الخصائص الموسعة.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// قراءة السمات الموسعة للمهام
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // قراءة المعلومات العامة حول الخاصية الموسعة
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### انظر أيضًا

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


