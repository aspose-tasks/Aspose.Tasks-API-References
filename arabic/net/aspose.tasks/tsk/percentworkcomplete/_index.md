---
title: "Tsk.PercentWorkComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الحالة الحالية للمهمة معبرًا عنها كنسبة مئوية للعمل الذي تم إنجازه"
type: docs
weight: 890
url: /ar/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

الحالة الحالية للمهمة معبرًا عنها كنسبة مئوية من العمل الذي تم إكماله.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


