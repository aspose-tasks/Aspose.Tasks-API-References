---
title: "Tsk.CommitmentStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تاريخ بدء التسليم. القراءة مدعومة فقط لتنسيق XML"
type: docs
weight: 180
url: /ar/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

تاريخ البدء للتسليم. القراءة مدعومة فقط لتنسيق XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


