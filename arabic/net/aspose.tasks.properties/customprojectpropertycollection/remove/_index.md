---
title: "CustomProjectPropertyCollection.Remove"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CustomProjectPropertyCollection. تزيل خاصية بالاسم المحدد من المجموعة"
type: docs
weight: 50
url: /ar/net/aspose.tasks.properties/customprojectpropertycollection/remove/
---
## CustomProjectPropertyCollection.Remove method

يزيل خاصية بالاسم المحدد من المجموعة.

```csharp
public bool Remove(string name)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم الخاصية غير حساس لحالة الأحرف. |

### قيمة الإرجاع

صحيح إذا تم العثور على العنصر وإزالته بنجاح؛ وإلا، خطأ.

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


