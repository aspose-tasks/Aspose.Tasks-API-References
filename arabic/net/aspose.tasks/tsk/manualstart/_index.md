---
title: "Tsk.ManualStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد بدء المهمة المجدول يدويًا"
type: docs
weight: 800
url: /ar/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

يحدد تاريخ البدء المجدول يدويًا للمهمة.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


