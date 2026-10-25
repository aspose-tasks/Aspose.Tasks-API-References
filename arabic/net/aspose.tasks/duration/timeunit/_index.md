---
title: "Duration.TimeUnit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Duration. تحصل على نوع وحدة الوقت لهذا الكائن. نوع وحدة الوقت لنسخة Duration هذه."
type: docs
weight: 50
url: /ar/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

يحصل على نوع وحدة الوقت لهذا الكائن. نوع وحدة الوقت لهذا الكائن Duration.

```csharp
public TimeUnitType TimeUnit { get; }
```

## الأمثلة

يعرض كيفية تحديث مدة المهام.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// احصل على مهمة
var task1 = project.RootTask.Children.GetById(1);

// حدّث مدة المهمة
var duration1 = task1.Get(Tsk.Duration);

// أضف يومًا واحدًا إلى المهمة 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// عيّن مدة جديدة للمهمة
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// احصل على مهمة أخرى
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// غيّر المدة باستخدام نوع وحدة الوقت الفعلية
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// عيّن مدة جديدة للمهمة
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### انظر أيضًا

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


