---
title: "Tsk.LevelingDelay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت الذي يجب تأخير المهمة فيه عن تاريخ بدايتها المبكر بسبب موازنة الموارد."
type: docs
weight: 770
url: /ar/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

الوقت الذي ستتأخر فيه المهمة عن تاريخ بدايتها المبكر بسبب تسوية الموارد.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


