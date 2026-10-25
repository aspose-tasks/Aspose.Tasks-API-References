---
title: "Tsk.IsRecurring"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة جزءًا من سلسلة مهام متكررة"
type: docs
weight: 670
url: /ar/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

يحدد ما إذا كانت المهمة جزءًا من سلسلة مهام متكررة.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


