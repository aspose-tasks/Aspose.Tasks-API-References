---
title: "ChildTasksCollector.Tasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ChildTasksCollector. تحصل على قائمة بمهام الكائنات الفرعية المجمعة"
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

يحصل على قائمة بالكائنات الفرعية المجمعة (المهام).

```csharp
public List<Task> Tasks { get; }
```

## الأمثلة

يوضح كيفية التكرار على جميع المهام في مشروع كقائمة عادية.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


