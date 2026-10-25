---
title: "الفئة DailyWorkRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.DailyWorkRepetition. تمثل فئة للتكرارات في نمط التكرار اليومي بناءً على أيام العمل"
type: docs
weight: 420
url: /ar/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

يمثل فئة للتكرارات في نمط التكرار اليومي بناءً على أيام العمل.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | ينشئ مثيلاً جديداً للفئة `DailyWorkRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | يحصل أو يعيّن عدد الأيام الذي يمثل الفاصل بالأيام بين الوقائع. |

## الأمثلة

يوضح كيفية العمل مع تكرارات نمط تكرار العمل اليومي أثناء إنشاء مهام متكررة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// العمل مع المشروع أكثر...
// ...
```

### انظر أيضًا

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


