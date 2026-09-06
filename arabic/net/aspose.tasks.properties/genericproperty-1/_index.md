---
title: "بنية GenericPropertyTKey"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "بنية Aspose.Tasks.Properties.GenericProperty1TKey. تمثل خاصية حاوية"
type: docs
weight: 1570
url: /ar/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

يمثل خاصية حاوية.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| معامل | الوصف |
| --- | --- |
| TKey | نوع قيمة الخاصية. |

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | ينشئ مثيلاً جديداً للبنية `GenericProperty`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | يحصل على اسم الخاصية. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | يحصل على قيمة الخاصية. |

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


