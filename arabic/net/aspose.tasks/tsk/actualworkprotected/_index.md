---
title: "Tsk.ActualWorkProtected"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة التي يتم فيها حماية العمل الفعلي. القراءة مدعومة فقط لتنسيق XML"
type: docs
weight: 100
url: /ar/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

المدة التي يتم فيها حماية العمل الفعلي. القراءة مدعومة فقط لتنسيق XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


