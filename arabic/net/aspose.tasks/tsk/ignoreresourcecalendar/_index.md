---
title: "Tsk.IgnoreResourceCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت جدولة المهمة تأخذ في الاعتبار تقاويم الموارد المخصصة للمهمة"
type: docs
weight: 530
url: /ar/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

يحدد ما إذا كان جدولة المهمة يأخذ في الاعتبار تقاويم الموارد المُعيّنة للمهمة.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


