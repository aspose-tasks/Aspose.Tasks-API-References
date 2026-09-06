---
title: "الفئة DailyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.DailyRecurrencePattern. تمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة يوميًا في مشروع"
type: docs
weight: 400
url: /ar/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة يوميًا في مشروع.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | ينشئ مثيلًا جديدًا للفئة `DailyRecurrencePattern`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | يحصل أو يحدد نطاق التكرار. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | يحصل أو يحدد نمط التكرارات في نمط التكرار اليومي. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


