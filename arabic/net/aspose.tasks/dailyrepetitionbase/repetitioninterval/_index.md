---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية DailyRepetitionBase. تحصل أو تعين عدد الأيام الذي يمثل الفاصل بالأيام بين التكرارات"
type: docs
weight: 10
url: /ar/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

يحصل أو يعيّن عدد الأيام الذي يمثل الفاصل بالأيام بين الوقائع.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


