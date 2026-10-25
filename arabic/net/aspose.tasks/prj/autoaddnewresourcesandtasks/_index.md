---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يتم إضافة الموارد أو المهام الجديدة تلقائيًا إلى مجموعة الموارد أو المهام"
type: docs
weight: 50
url: /ar/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

يحدد ما إذا تم إضافة الموارد أو المهام الجديدة تلقائيًا إلى مجموعة الموارد أو المهام.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.AutoAddNewResourcesAndTasks.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


