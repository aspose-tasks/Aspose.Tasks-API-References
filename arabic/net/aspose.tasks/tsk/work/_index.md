---
title: "Tsk.Work"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. إجمالي الوقت المجدول للمهمة لجميع الموارد المعينة"
type: docs
weight: 1150
url: /ar/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

الوقت الإجمالي المجدول للمهمة لجميع الموارد المعينة.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


