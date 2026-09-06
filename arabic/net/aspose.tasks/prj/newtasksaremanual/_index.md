---
title: "Prj.NewTasksAreManual"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت المهام الجديدة تُنشأ يدويًا"
type: docs
weight: 550
url: /ar/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

يحدد ما إذا كانت المهام الجديدة تُنشأ يدويًا.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


