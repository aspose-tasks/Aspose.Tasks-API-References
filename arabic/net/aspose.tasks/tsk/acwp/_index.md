---
title: "Tsk.ACWP"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التكاليف المتكبدة للعمل المنجز بالفعل على مهمة حتى تاريخ حالة المشروع أو تاريخ اليوم"
type: docs
weight: 110
url: /ar/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

التكاليف المتكبدة للعمل الذي تم إنجازه بالفعل على مهمة، حتى تاريخ حالة المشروع أو تاريخ اليوم.

```csharp
public static readonly Key<double, TaskKey> ACWP;
```

## الأمثلة

يوضح كيفية قراءة قيم تكلفة المهمة.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


