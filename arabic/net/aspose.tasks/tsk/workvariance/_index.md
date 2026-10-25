---
title: "Tsk.WorkVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الفرق بين العمل الأساسي للمهمة والعمل المجدول حاليًا"
type: docs
weight: 1160
url: /ar/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

الفرق بين العمل الأساسي للمهمة والعمل المجدول حاليًا.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


