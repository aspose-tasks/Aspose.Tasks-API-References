---
title: "Tsk.IsEstimated"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة مقدرة."
type: docs
weight: 580
url: /ar/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

يحدد ما إذا كانت المهمة مقدرة.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## الأمثلة

يوضح كيفية العثور على المهام المقدرة و/أو مهام العلامة

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// التكرار على المهام المجمعة
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


