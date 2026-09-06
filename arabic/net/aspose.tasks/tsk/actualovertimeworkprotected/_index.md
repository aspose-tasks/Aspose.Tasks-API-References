---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة التي يتم فيها حماية العمل الإضافي الفعلي"
type: docs
weight: 70
url: /ar/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

المدة التي يتم فيها حماية العمل الإضافي الفعلي.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## الأمثلة

يظهر كيفية قراءة/كتابة الخاصية Tsk.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


