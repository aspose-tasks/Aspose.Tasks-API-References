---
title: "Tsk.PhysicalPercentComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. قيمة النسبة المكتملة التي يمكن استخدامها كبديل لحساب التكلفة الموازنة للعمل المنجز (BCWP)."
type: docs
weight: 900
url: /ar/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

قيمة النسبة المئوية المكتملة التي يمكن استخدامها كبديل لحساب تكلفة العمل المنجز وفق الميزانية (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


