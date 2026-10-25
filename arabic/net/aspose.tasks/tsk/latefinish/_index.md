---
title: "Tsk.LateFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. أحدث تاريخ يمكن للمهمة أن تنتهي فيه دون تأخير انتهاء المشروع."
type: docs
weight: 730
url: /ar/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

أحدث تاريخ يمكن للمهمة أن تنتهي فيه دون تأخير انتهاء المشروع.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


