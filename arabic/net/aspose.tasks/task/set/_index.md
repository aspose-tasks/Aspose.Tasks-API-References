---
title: "Task.Set"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تقوم بربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية"
type: docs
weight: 1410
url: /ar/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحددة. [`Tsk`](../../tsk/) للحصول على مفتاح الخاصية. |
| القيمة | القيمة. |

## الأمثلة

يعرض كيفية الحصول/تعيين خصائص المهمة.

```csharp
var project = new Project();

// إضافة مهمة وتعيين خصائص المهمة
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


