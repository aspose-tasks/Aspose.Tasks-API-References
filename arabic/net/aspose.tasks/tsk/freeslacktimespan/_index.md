---
title: "Tsk.FreeSlackTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت الذي يمكن تأخير المهمة فيه دون تأخير أي مهام لاحقة."
type: docs
weight: 450
url: /ar/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

الوقت الذي يمكن فيه تأخير المهمة دون تأخير أي مهام لاحقة.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## الأمثلة

يعرض كيفية قراءة الخاصية Tsk.FreeSlackTimeSpan. الخاصية محسوبة، لذا عادةً لا حاجة لتعيينها صراحةً.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


