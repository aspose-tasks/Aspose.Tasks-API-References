---
title: "Tsk.FinishSlackTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة بين تاريخ الانتهاء المبكر وتاريخ الانتهاء المتأخر"
type: docs
weight: 400
url: /ar/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

المدة بين تاريخ الانتهاء المبكر وتاريخ الانتهاء المتأخر.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## الأمثلة

يظهر كيفية قراءة خاصية Tsk.FinishSlackTimeSpan. الخاصية محسوبة، لذا عادةً لا يلزم تعيينها يدويًا.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


