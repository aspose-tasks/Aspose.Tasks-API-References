---
title: "Tsk.ActualCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التكاليف المتكبدة للعمل الذي قام به الموارد بالفعل على مهامهم بالإضافة إلى أي تكاليف مسجلة أخرى مرتبطة بالمهمة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

التكاليف المتكبدة للعمل الذي تم إنجازه بالفعل من قبل الموارد على مهامهم، إلى جانب أي تكاليف مسجلة أخرى مرتبطة بالمهمة.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


