---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ChildTasksCollector. يهيئ مثيلاً جديداً من الفئة ChildTasksCollector"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

يهيئ مثيلاً جديداً من الفئة [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


