---
title: "Project.BuiltInProps"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على مجموعة خصائص المشروع المدمجة"
type: docs
weight: 100
url: /ar/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

يحصل على مجموعة الخصائص المدمجة للمشروع.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
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

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


