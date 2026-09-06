---
title: "Tsk.HideBar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان شريط جانت للمهمة مخفيًا عند عرضه في Microsoft Project."
type: docs
weight: 480
url: /ar/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

يحدد ما إذا كان شريط جانت للمهمة مخفيًا عند عرضه في Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


