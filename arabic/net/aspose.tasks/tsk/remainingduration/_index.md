---
title: "Tsk.RemainingDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت المطلوب لإكمال الجزء غير المكتمل من المهمة"
type: docs
weight: 960
url: /ar/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

الوقت المطلوب لإكمال الجزء غير المكتمل من المهمة.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


