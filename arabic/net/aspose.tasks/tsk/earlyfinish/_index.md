---
title: "Tsk.EarlyFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. أقدم تاريخ يمكن أن تنتهي فيه المهمة بناءً على تواريخ الانتهاء المبكرة للمهام السابقة واللاحقة، والقيود الأخرى، وأي تأخير في التوازن"
type: docs
weight: 330
url: /ar/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

أقرب تاريخ يمكن أن تنتهي فيه المهمة، استنادًا إلى تواريخ الانتهاء المبكرة للمهام السابقة واللاحقة، والقيود الأخرى، وأي تأخير في التسوية.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


