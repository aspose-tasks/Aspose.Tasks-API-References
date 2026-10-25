---
title: "فئة Property"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Properties.Property. تمثل فئة أساسية لخاصية"
type: docs
weight: 1580
url: /ar/net/aspose.tasks.properties/property/
---
## Property class

يمثل فئة أساسية لخاصية.

```csharp
public abstract class Property
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | يحصل على اسم الخاصية. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | يحصل أو يضبط قيمة الخاصية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | يرجع قيمة الخاصية كسلسلة. |

## الأمثلة

يوضح كيفية قراءة خصائص المشروع المدمجة.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// التكرار على مجموعة الخصائص المدمجة
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### انظر أيضًا

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


