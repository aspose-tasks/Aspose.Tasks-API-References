---
title: "Tsk.IsEffortDriven"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت جدولة المهمة تعتمد على الجهد"
type: docs
weight: 570
url: /ar/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

يحدد ما إذا كانت جدولة المهمة تعتمد على الجهد.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## الأمثلة

يعرض كيفية العثور على المهام الحرجة و/أو التي تعتمد على الجهد.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


