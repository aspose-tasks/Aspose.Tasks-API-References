---
title: "Tsk.RemainingWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام"
type: docs
weight: 990
url: /ar/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

الوقت المتبقي المطلوب لإكمال مهمة أو مجموعة مهام.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


