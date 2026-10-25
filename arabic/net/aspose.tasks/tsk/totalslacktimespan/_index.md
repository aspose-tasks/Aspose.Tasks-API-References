---
title: "Tsk.TotalSlackTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. الوقت الذي يمكن تأخير تاريخ انتهاء المهمة فيه دون تأخير تاريخ انتهاء المشروع."
type: docs
weight: 1090
url: /ar/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

الوقت الذي يمكن تأخير تاريخ انتهاء المهمة فيه دون تأخير تاريخ انتهاء المشروع.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## الأمثلة

يعرض كيفية قراءة الخاصية Tsk.TotalSlackTimeSpan. الخاصية محسوبة، لذا عادةً لا حاجة لتعيينها صراحةً.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


