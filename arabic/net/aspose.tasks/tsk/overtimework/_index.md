---
title: "Tsk.OvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. مقدار العمل الإضافي المجدول الذي سيؤديه جميع الموارد المعينة للمهمة"
type: docs
weight: 870
url: /ar/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

كمية العمل الإضافي المجدولة التي سيؤديها جميع الموارد المخصصة للمهمة.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## الأمثلة

يوضح كيفية قراءة العمل الإضافي للمهمة.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// قراءة العمل الإضافي ونسبة الإنجاز للمهام
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // تعيين النسبة المكتملة
    task.Set(Tsk.PercentComplete, 100);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


