---
title: "Prj.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. اسم المشروع"
type: docs
weight: 540
url: /ar/net/aspose.tasks/prj/name/
---
## Prj.Name field

اسم المشروع.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## الأمثلة

يوضح كيفية قراءة/كتابة اسم المشروع.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


