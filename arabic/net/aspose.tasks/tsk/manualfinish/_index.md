---
title: "Tsk.ManualFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد الانتهاء المجدول يدويًا لمهمة"
type: docs
weight: 790
url: /ar/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

يحدد تاريخ الانتهاء المجدول يدويًا للمهمة.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


