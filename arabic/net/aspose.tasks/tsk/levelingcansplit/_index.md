---
title: "Tsk.LevelingCanSplit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت وظيفة تسوية الموارد يمكن أن تتسبب في تقسيم العمل المتبقي على هذه المهمة"
type: docs
weight: 760
url: /ar/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

يحدد ما إذا كانت وظيفة تسوية الموارد يمكنها إحداث تقسيمات على العمل المتبقي في هذه المهمة.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


