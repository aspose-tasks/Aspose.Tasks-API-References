---
title: "الفئة EndAfterRecurrenceRange"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.EndAfterRecurrenceRange. تمثل نطاق التكرار للمهمة المتكررة الذي يحده عدد مرات التكرار"
type: docs
weight: 500
url: /ar/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

يمثل نطاق التكرار للمهمة المتكررة الذي يحده عدد مرات التكرار.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | يُهيئ نسخة جديدة من الفئة `EndAfterRecurrenceRange`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | يحصل أو يعيّن عدد مرات التكرار التي تحدّ نطاق التكرار للمهمة المتكررة. |
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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


