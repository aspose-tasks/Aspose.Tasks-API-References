---
title: "Tsk.FinishVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت الذي يمثل الفرق بين تاريخ الانتهاء الأساسي للمهمة أو التعيين وتاريخ الانتهاء الحالي"
type: docs
weight: 420
url: /ar/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

الوقت الذي يمثل الفرق بين تاريخ الانتهاء الأساسي للمهمة أو التعيين وتاريخ الانتهاء الحالي.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


