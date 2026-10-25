---
title: "Tsk.ActualOvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. كمية العمل الإضافي الفعلية التي أُجريت بالفعل من قبل الموارد المخصصة للمهام."
type: docs
weight: 60
url: /ar/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

الكمية الفعلية للعمل الإضافي الذي تم إنجازه بالفعل من قبل الموارد المخصصة للمهمات.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


