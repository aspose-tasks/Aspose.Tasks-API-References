---
title: "Tsk.Type"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. نوع المهمة"
type: docs
weight: 1100
url: /ar/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

نوع المهمة.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


