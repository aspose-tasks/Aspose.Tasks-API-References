---
title: "Tsk.RemainingCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المصروف المجدول المتبقي الذي سيتكبد عند إكمال العمل المجدول المتبقي"
type: docs
weight: 950
url: /ar/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

النفقات المجدولة المتبقية التي ستُتحمل عند إكمال العمل المجدول المتبقي.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
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


