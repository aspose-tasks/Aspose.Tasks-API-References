---
title: "الفئة PropertyKeyedCollectionT"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Properties.PropertyKeyedCollection1T. فئة أساسية لمجموعة الخصائص"
type: docs
weight: 1600
url: /ar/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

فئة أساسية لمجموعة من الخصائص.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| معامل | الوصف |
| --- | --- |
| T | نوع الخاصية. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | يحصل على عدد الخصائص في المجموعة. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | يحصل على الخاصية المرتبطة بالمفتاح المحدد. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | يحصل على مجموعة جميع أسماء الخصائص. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | ينشئ خاصية مخصصة جديدة. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | يحدد ما إذا كان [`PropertyCollection`](../propertycollection-1/) يحتوي على خاصية بالاسم المحدد. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


