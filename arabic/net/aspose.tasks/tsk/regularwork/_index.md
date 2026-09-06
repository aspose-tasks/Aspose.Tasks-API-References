---
title: "Tsk.RegularWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. إجمالي مقدار العمل غير الإضافي المجدول الذي ستقوم الموارد بأدائه"
type: docs
weight: 940
url: /ar/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

إجمالي كمية العمل غير الإضافي المجدول الذي سيؤديه الموارد.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


