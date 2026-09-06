---
title: "Tsk.WBSLevel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المستوى الأيمن من مستويات WBS للمهمة"
type: docs
weight: 1140
url: /ar/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

المستوى الأيمن لهيكل تقسيم العمل (WBS) للمهمة.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
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


