---
title: "Tsk.RemainingOvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. مقدار الوقت الإضافي المجدول المتبقي"
type: docs
weight: 980
url: /ar/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

كمية الوقت المتبقي المجدول للعمل الإضافي.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


