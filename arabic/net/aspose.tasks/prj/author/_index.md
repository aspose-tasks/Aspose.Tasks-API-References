---
title: "Prj.Author"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. مؤلف المشروع"
type: docs
weight: 40
url: /ar/net/aspose.tasks/prj/author/
---
## Prj.Author field

مؤلف المشروع.

```csharp
public static readonly Key<string, PrjKey> Author;
```

## الأمثلة

يظهر كيفية تعيين معلومات تعريف المشروع.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// تعيين معلومات المشروع
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


