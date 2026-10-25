---
title: "الفئة CustomProjectProperty"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Properties.CustomProjectProperty. تمثّل خاصية مخصصة"
type: docs
weight: 1540
url: /ar/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

يمثل خاصية مخصصة.

```csharp
public sealed class CustomProjectProperty : Property
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | يحصل على اسم الخاصية. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | يحصل على نوع الخاصية. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | يحصل أو يضبط قيمة الخاصية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | يرجع قيمة الخاصية كسلسلة. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


