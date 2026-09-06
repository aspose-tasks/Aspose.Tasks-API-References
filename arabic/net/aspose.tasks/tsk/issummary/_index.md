---
title: "Tsk.IsSummary"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة مهمة ملخص"
type: docs
weight: 720
url: /ar/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

يحدد ما إذا كانت المهمة مهمة ملخص.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


