---
title: "Duration.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Duration. تضيف المدة المحددة إلى هذه المدة."
type: docs
weight: 60
url: /ar/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

يضيف المدة المحددة إلى هذه المدة.

```csharp
public Duration Add(Duration d)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| d | Duration | المدة المحددة [`Duration`](../) لإضافتها إلى هذه النسخة. |

### قيمة الإرجاع

كائن مدة جديد يمثل قيمة هذه المثيلة بالإضافة إلى قيمة المدة المحددة.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

يضيف القيمة المزدوجة المحددة إلى هذه المدة.

```csharp
public Duration Add(double val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Double | القيمة المزدوجة المحددة لإضافتها إلى هذه المثيلة. |

### قيمة الإرجاع

كائن مدة جديد يمثل قيمة هذه المثيلة بالإضافة إلى قيمة المدة المحددة.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


