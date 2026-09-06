---
title: "EndAfterRecurrenceRange.OccurrenceNumber"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية EndAfterRecurrenceRange. يحصل أو يعيّن عدد مرات التكرار التي تحدّ حدود نطاق التكرار للمهمة المتكررة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/endafterrecurrencerange/occurrencenumber/
---
## EndAfterRecurrenceRange.OccurrenceNumber property

يحصل أو يعيّن عدد مرات التكرار التي تحدّ نطاق التكرار للمهمة المتكررة.

```csharp
public int OccurrenceNumber { get; set; }
```

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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


