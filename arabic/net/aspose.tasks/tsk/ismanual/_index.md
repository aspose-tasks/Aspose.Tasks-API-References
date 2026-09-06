---
title: "Tsk.IsManual"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت المهمة مجدولة يدويًا"
type: docs
weight: 610
url: /ar/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

يحدد ما إذا كانت المهمة مجدولة يدويًا.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


