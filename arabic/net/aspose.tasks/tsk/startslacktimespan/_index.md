---
title: "Tsk.StartSlackTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة بين تواريخ البدء المبكر والبدء المتأخر"
type: docs
weight: 1020
url: /ar/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

المدة بين تاريخ البدء المبكر وتاريخ البدء المتأخر.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## الأمثلة

يعرض كيفية قراءة خاصية Tsk.StartSlackTimeSpan. الخاصية محسوبة، لذا عادة لا يلزم تعيينها يدويًا.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


