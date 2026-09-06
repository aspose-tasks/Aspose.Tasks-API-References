---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب تحديث المهام اليدوية عند تعديل الروابط"
type: docs
weight: 770
url: /ar/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

يحدد ما إذا كان يجب تحديث المهام اليدوية عندما تم تعديل الروابط.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.UpdateManuallyScheduledTasksWhenEditingLinks.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


