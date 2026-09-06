---
title: "Tsk.OvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. إجمالي تكلفة العمل الإضافي لمهمة معينة أو لمورد على جميع المهام المخصصة أو لتعيين المورد."
type: docs
weight: 860
url: /ar/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

إجمالي تكلفة العمل الإضافي للمهمة، أو للموارد على جميع المهام المخصصة، أو لتخصيص المورد.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


