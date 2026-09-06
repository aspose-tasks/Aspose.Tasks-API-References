---
title: "Tsk.ActualWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. مقدار العمل الذي تم إنجازه بالفعل من قبل الموارد المخصصة للمهام"
type: docs
weight: 90
url: /ar/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

كمية العمل التي تم إنجازها بالفعل من قبل الموارد المخصصة للمهمات.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


