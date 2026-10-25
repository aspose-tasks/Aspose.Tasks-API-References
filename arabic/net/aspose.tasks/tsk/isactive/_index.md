---
title: "Tsk.IsActive"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة نشطة. المهام غير النشطة لم تعد تؤثر على المهام الأخرى أو على جدول المشروع العام."
type: docs
weight: 550
url: /ar/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

يحدد ما إذا كانت المهمة نشطة. المهام غير النشطة لم تعد تؤثر على المهام الأخرى أو جدول المشروع العام.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


