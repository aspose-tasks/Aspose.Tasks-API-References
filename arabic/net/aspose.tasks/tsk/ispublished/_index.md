---
title: "Tsk.IsPublished"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان يجب نشر المهمة الحالية إلى خادم Project Server مع باقي المشروع"
type: docs
weight: 660
url: /ar/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

يحدد ما إذا كان يجب نشر المهمة الحالية إلى Project Server مع باقي المشروع.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


