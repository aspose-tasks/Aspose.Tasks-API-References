---
title: "Task.Get"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُرجع القيمة التي تم ربط الخاصية بها في هذا الحاوية"
type: docs
weight: 1340
url: /ar/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحددة. [`Tsk`](../../tsk/) للحصول على مفتاح الخاصية. |

### قيمة الإرجاع

القيمة التي تم تعيين الخاصية إليها في هذا الحاوية.

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


