---
title: "Tsk.FixedCostAccrual"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد الخيارات لكيفية ومتى يتم تحميل التكاليف الثابتة أو تراكمها إلى تكلفة المهمة"
type: docs
weight: 440
url: /ar/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

يحدد الخيارات لكيفية ومتى يتم تحميل التكاليف الثابتة، أو تراكمها، إلى تكلفة المهمة.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


