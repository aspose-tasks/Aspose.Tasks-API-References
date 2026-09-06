---
title: "Tsk.Calendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. تقويم المهمة"
type: docs
weight: 160
url: /ar/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

تقويم المهمة.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## الأمثلة

يوضح كيفية قراءة/كتابة تقاويم المهام.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// إنشاء تقويم وتعيينه للمهمة
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع العناصر المتداخلة
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


