---
title: "Tsk.BCWP"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. القيمة التراكمية لنسبة إكمال المهمة مضروبة في تكاليف الخط الأساسي المجدولة زمنياً"
type: docs
weight: 120
url: /ar/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

القيمة التراكمية لنسبة إنجاز المهمة مضروبة في تكاليف الخط الأساسي المتدرجة زمنياً.

```csharp
public static readonly Key<double, TaskKey> BCWP;
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


