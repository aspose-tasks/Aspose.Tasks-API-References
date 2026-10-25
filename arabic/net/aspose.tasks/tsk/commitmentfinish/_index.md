---
title: "Tsk.CommitmentFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تاريخ الانتهاء للتسليم.  القراءة مدعومة فقط لتنسيق XML"
type: docs
weight: 170
url: /ar/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

تاريخ الانتهاء للتسليم. القراءة مدعومة فقط لتنسيق XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


