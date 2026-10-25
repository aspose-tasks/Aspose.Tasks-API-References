---
title: "Tsk.OutlineLevel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. مستوى المخطط للمهمة"
type: docs
weight: 840
url: /ar/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

مستوى المخطط للمهمة.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## الأمثلة

يظهر كيفية قراءة خصائص مخطط المهمة.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


