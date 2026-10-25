---
title: "Tsk.Created"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التاريخ الذي تم فيه إنشاء المهمة."
type: docs
weight: 250
url: /ar/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

التاريخ الذي تم فيه إنشاء المهمة.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


