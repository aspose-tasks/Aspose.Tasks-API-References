---
title: "Tsk.LateStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. أحدث تاريخ يمكن للمهمة أن تبدأ فيه دون تأخير انتهاء المشروع"
type: docs
weight: 740
url: /ar/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

أحدث تاريخ يمكن للمهمة أن تبدأ فيه دون تأخير انتهاء المشروع.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


