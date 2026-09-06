---
title: "Tsk.EarlyStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. أقرب تاريخ يمكن أن تبدأ فيه المهمة بناءً على تواريخ البدء المبكرة للمهام السابقة واللاحقة وغيرها من القيود"
type: docs
weight: 340
url: /ar/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

أقرب تاريخ يمكن أن يبدأ فيه المهمة، استنادًا إلى تواريخ البدء المبكرة للمهام السابقة واللاحقة والقيود الأخرى.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


