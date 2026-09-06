---
title: "Tsk.PreleveledStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تاريخ بدء المهمة كما كان قبل إجراء تسوية الموارد"
type: docs
weight: 920
url: /ar/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

تاريخ البدء للمهمة كما كان قبل إجراء تسوية الموارد.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


