---
title: "Tsk.Deadline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تاريخ الهدف الذي يشير إلى موعد إكمال المهمة."
type: docs
weight: 270
url: /ar/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

تاريخ هدف يشير إلى موعد إكمال المهمة.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


