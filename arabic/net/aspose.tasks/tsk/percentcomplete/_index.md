---
title: "Tsk.PercentComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الحالة الحالية لمهمة معبرًا عنها كنسبة مئوية من مدة المهمة التي تم إكمالها"
type: docs
weight: 880
url: /ar/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

الحالة الحالية للمهمة، معبرًا عنها كنسبة مئوية من مدة المهمة التي تم إكمالها.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## الأمثلة

يظهر كيفية تغيير تقدم المهمة عن طريق تحديث نسبة إكمال المهمة.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// الوصول إلى المهام وعرض نسبة الإنجاز
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


