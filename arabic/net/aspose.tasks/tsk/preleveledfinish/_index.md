---
title: "Tsk.PreleveledFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تاريخ الانتهاء للمهمة كما كان قبل إجراء تسوية الموارد."
type: docs
weight: 910
url: /ar/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

تاريخ الانتهاء للمهمة كما كان قبل إجراء تسوية الموارد.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


