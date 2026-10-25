---
title: "Tsk.WBS"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. رموز هيكل تقسيم العمل WBS"
type: docs
weight: 1130
url: /ar/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

رموز هيكل تقسيم العمل (WBS).

```csharp
public static readonly Key<string, TaskKey> WBS;
```

## الأمثلة

يظهر كيفية قراءة رموز WBS للمهمة.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


