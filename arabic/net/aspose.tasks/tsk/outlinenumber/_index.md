---
title: "Tsk.OutlineNumber"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الرقم الذي يمثل موقع المهمة في هيكل المخطط الهرمي"
type: docs
weight: 850
url: /ar/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

الرقم الذي يمثل موضع المهمة في هيكل المخطط الهرمي.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
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


