---
title: "Tsk.IsExpanded"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت مهمة الملخص موسعة أم لا في عرض مخطط جانت"
type: docs
weight: 590
url: /ar/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

يحدد ما إذا كانت مهمة الملخص موسعة أم لا في عرض مخطط جانت.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


