---
title: "الهيكل Duration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الهيكل Aspose.Tasks.Duration. يمثل المدة في مشروع."
type: docs
weight: 470
url: /ar/net/aspose.tasks/duration/
---
## Duration structure

يمثل المدة في مشروع.

```csharp
public struct Duration : IEquatable<Duration>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت منقضية. العلامة التي تحدد ما إذا كان هذا المثيل من Duration منقضيًا. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت وحدة الوقت مقدرة. العلامة التي تحدد ما إذا كان هذا المثيل من Duration مقدّرًا. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | يحصل على كائن [`TimeSpan`](./timespan/) لهذا الكائن Duration. كائن TimeSpan لهذا الكائن Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | يحصل على نوع وحدة الوقت لهذا الكائن. نوع وحدة الوقت لهذا الكائن Duration. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | يحوّل السلسلة المحددة إلى كائن من بنية `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | يضيف القيمة المزدوجة المحددة إلى هذه المدة. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | يضيف المدة المحددة إلى هذه المدة. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | يحوّل كائن Duration إلى مدة أخرى بوحدات زمنية محددة. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | يعيد قيمة رمز التجزئة لهذا الكائن. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | يطرح القيمة المزدوجة المحددة من كائن المدة هذا. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | يطرح المدة المحددة من كائن المدة هذا. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | يحوّل كائن Duration إلى قيمة Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | يعيد تمثيلًا نصيًا لهذا الكائن. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | يحلل سلسلة المدة بالتنسيق "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


