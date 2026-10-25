---
title: "Project.CustomProps"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. يحصل على مجموعة خصائص المشروع المخصصة"
type: docs
weight: 260
url: /ar/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

يحصل على مجموعة الخصائص المخصصة للمشروع.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## الأمثلة

يعرض كيفية قراءة خصائص ميتا المشروع (واجهة برمجة تطبيقات قديمة).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// الخصائص المخصصة متاحة عبر المجموعة ذات النوع المحدد
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// الخصائص المدمجة متاحة مباشرة
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// أو كعنصر من مجموعة الخصائص المدمجة
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### انظر أيضًا

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


