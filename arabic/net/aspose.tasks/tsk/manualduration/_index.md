---
title: "Tsk.ManualDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد المدة المجدولة يدويًا لمهمة"
type: docs
weight: 780
url: /ar/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

يحدد المدة المجدولة يدويًا للمهمة.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


