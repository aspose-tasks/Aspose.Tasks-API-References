---
title: "Duration.Subtract"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تقوم بطرح المدة المحددة من نسخة هذه المدة."
type: docs
weight: 100
url: /ar/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

يطرح المدة المحددة من كائن المدة هذا.

```csharp
public Duration Subtract(Duration d)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| d | Duration | النسخة المحددة من [`Duration`](../) لطرحها من هذه النسخة. |

### قيمة الإرجاع

كائن مدة جديد يمثل قيمة هذه النسخة مطروحًا منها قيمة المدة المحددة.

## الأمثلة

يوضح كيفية تغيير مدة المهام.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// احصل على مهمة
var task1 = project.RootTask.Children.GetById(1);

// حدّث مدة المهمة
var duration1 = task1.Get(Tsk.Duration);

// اطرح يومًا واحدًا من المهمة 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// عيّن مدة جديدة للمهمة
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// احصل على مهمة أخرى
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// غيّر المدة باستخدام نوع وحدة الوقت الفعلية
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// عيّن مدة جديدة للمهمة
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

يطرح القيمة المزدوجة المحددة من كائن المدة هذا.

```csharp
public Duration Subtract(double val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Double | قيمة Double المحددة لطرحها من هذه النسخة. |

### قيمة الإرجاع

كائن مدة جديد يمثل قيمة هذه النسخة مطروحًا منها قيمة المدة المحددة.

## الأمثلة

يوضح كيفية تغيير مدة المهام.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// احصل على مهمة
var task1 = project.RootTask.Children.GetById(1);

// حدّث مدة المهمة
var duration1 = task1.Get(Tsk.Duration);

// اطرح يومًا واحدًا من المهمة 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// عيّن مدة جديدة للمهمة
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// احصل على مهمة أخرى
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// غيّر المدة باستخدام نوع وحدة الوقت الفعلية
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// عيّن مدة جديدة للمهمة
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


