---
title: "Tsk.StartVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت الذي يمثل الفرق بين تاريخ البدء الأساسي للمهمة أو التعيين وتاريخ البدء المجدول الحالي."
type: docs
weight: 1040
url: /ar/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

الوقت الذي يمثل الفرق بين تاريخ بدء الأساس لمهمة أو تعيين وتاريخ بدءها المجدول حاليًا.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


