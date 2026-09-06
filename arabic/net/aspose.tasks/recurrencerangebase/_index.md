---
title: "الفئة RecurrenceRangeBase"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.RecurrenceRangeBase. تمثل نطاق التكرار لمهمة متكررة."
type: docs
weight: 1710
url: /ar/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

يمثل نطاق التكرار للمهمة المتكررة.

```csharp
public abstract class RecurrenceRangeBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | يحصل أو يعيّن تاريخ بدء نطاق التكرار للمهمة المتكررة. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


