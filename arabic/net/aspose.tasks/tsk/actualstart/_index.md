---
title: "Tsk.ActualStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التاريخ والوقت الذي بدأت فيه المهمة فعليًا"
type: docs
weight: 80
url: /ar/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

التاريخ والوقت الذي بدأت فيه المهمة فعليًا.

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## الأمثلة

يعرض أن تواريخ المشروع تُعاد ضبطها في وضع التقييم.

```csharp
var project = new Project();

// إنشاء مهام جديدة
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


