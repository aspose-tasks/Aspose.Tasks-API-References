---
title: "Tsk.RemainingOvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. النفقات الإضافية المتبقية المجدولة للمهمة."
type: docs
weight: 970
url: /ar/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

المصروف المتبقي المجدول للعمل الإضافي للمهمة.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


