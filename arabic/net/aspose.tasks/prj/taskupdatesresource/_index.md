---
title: "Prj.TaskUpdatesResource"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت تحديثات المهام تُحدّث الموارد"
type: docs
weight: 710
url: /ar/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

يحدد ما إذا كانت تحديثات المهام تُحدّث الموارد.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.TaskUpdatesResource.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


