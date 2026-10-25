---
title: "Prj.SplitsInProgressTasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يمكن تقسيم المهام الجارية"
type: docs
weight: 650
url: /ar/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

يحدد ما إذا كان يمكن تقسيم المهام الجارية.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Prj.SplitsInProgressTasks.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


