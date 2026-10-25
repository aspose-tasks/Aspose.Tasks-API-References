---
title: "Tsk.DurationVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الفرق بين المدة الأساسية للمهمة والمدة الإجمالية للتقدير الحالي للمهمة."
type: docs
weight: 320
url: /ar/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

الفرق بين مدة الأساس للمهمة والمدة الإجمالية (التقدير الحالي) للمهمة.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


