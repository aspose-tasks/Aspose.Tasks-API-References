---
title: "Tsk.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. اسم المهمة"
type: docs
weight: 810
url: /ar/net/aspose.tasks/tsk/name/
---
## Tsk.Name field

اسم المهمة.

```csharp
public static readonly Key<string, TaskKey> Name;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خصائص المهمة.

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
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


