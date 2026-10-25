---
title: "Tsk.DurationText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يُرجع نص مدة المهمة"
type: docs
weight: 310
url: /ar/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

يعيد نص مدة المهمة.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


