---
title: "Tsk.Priority"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. مستوى الأهمية الممنوح للمهمة والذي بدوره يشير إلى مدى إمكانية تأخير أو تقسيم المهمة أو التعيين أثناء تسوية الموارد"
type: docs
weight: 930
url: /ar/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

مستوى الأهمية الممنوح للمهمة، والذي بدوره يشير إلى مدى سهولة تأخير أو تقسيم المهمة أو التخصيص أثناء تسوية الموارد.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## الأمثلة

يعرض كيفية قراءة أولوية المهمة.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// عرض الأولويات لجميع المهام
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


