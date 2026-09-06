---
title: "Tsk.CostVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الفرق بين التكلفة الأساسية والتكلفة الإجمالية لمورد المهمة أو التعيين"
type: docs
weight: 240
url: /ar/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

الفرق بين تكلفة الأساس والتكلفة الإجمالية للمهمة أو المورد أو التعيين.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


