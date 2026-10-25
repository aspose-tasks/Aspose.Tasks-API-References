---
title: "التعداد CustomPropertyType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Properties.CustomPropertyType. يمثل تعدادًا لنوع خاصية مخصصة"
type: docs
weight: 1560
url: /ar/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

يمثل تعداد نوع الخاصية المخصصة.

```csharp
public enum CustomPropertyType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | الخاصية ليس لها نوع. |
| String | `1` | الخاصية هي قيمة نصية. |
| DateTime | `2` | الخاصية هي قيمة تاريخ ووقت. |
| Number | `3` | الخاصية هي عدد صحيح. |
| Boolean | `4` | الخاصية هي قيمة منطقية. |

## الأمثلة

يعرض كيفية العمل مع مجموعات خصائص المشروع المخصصة.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// لنضيف خصائص مخصصة جديدة
// المجموعة تدعم الأنواع Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// الخصائص المخصصة متاحة عبر المجموعة ذات النوع المحدد
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// احصل على قيمة خاصية مخصصة
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// تكرار عبر أسماء الخصائص المخصصة
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// يمكن حذف قيمة باستخدام مفتاح نصي
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// أو يمكن للمرء مسح المجموعة بالكامل
project.CustomProps.Clear();
```

### انظر أيضًا

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


