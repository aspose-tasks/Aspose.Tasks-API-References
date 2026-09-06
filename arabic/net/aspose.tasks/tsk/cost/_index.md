---
title: "Tsk.Cost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التكلفة الإجمالية المجدولة أو المتوقعة للمهمة بناءً على التكاليف التي تم تكبدها بالفعل للعمل الذي قام به الموارد المعينة للمهمة بالإضافة إلى التكاليف المخططة للعمل المتبقي"
type: docs
weight: 230
url: /ar/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

التكلفة الإجمالية المجدولة أو المتوقعة للمهمة بناءً على التكاليف التي تم تكبدها بالفعل للعمل الذي قامت به الموارد المخصصة للمهمة، بالإضافة إلى التكاليف المخطط لها للعمل المتبقي.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
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


