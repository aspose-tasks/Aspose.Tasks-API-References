---
title: "Prj.AdminProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان المشروع مشروعًا إداريًا"
type: docs
weight: 20
url: /ar/net/aspose.tasks/prj/adminproject/
---
## Prj.AdminProject field

يحدد ما إذا كان المشروع مشروعًا إداريًا.

```csharp
public static readonly Key<NullableBool, PrjKey> AdminProject;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.AdminProject.

```csharp
var project = new Project();

project.Set(Prj.AdminProject, true);

Console.WriteLine("Admin Project: " + project.Get(Prj.AdminProject));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


