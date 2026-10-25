---
title: "Tsk.FixedCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يظهر أي نفقات غير مرتبطة بالموارد للمهمة"
type: docs
weight: 430
url: /ar/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

يعرض أي نفقات غير مرتبطة بالموارد للمهمة.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
```

## الأمثلة

يوضح كيفية قراءة تكاليف المهمة.

```csharp
var project = new Project();

// إضافة مهمة وتعيين التكلفة
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// عرض الخصائص المتعلقة بالتكلفة للمهمة
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


