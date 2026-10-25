---
title: "Tsk.ActualDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة الفعلية لوقت العمل للمهمة بناءً على المدة المجدولة والعمل المتبقي الحالي أو نسبة الإنجاز."
type: docs
weight: 30
url: /ar/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

الفترة الزمنية الفعلية للعمل لمهمة، بناءً على المدة المجدولة والعمل المتبقي الحالي أو نسبة الإنجاز.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## الأمثلة

يظهر كيفية قراءة الخصائص الفعلية للمهمة.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


