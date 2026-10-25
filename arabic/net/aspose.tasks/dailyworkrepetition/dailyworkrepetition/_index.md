---
title: "DailyWorkRepetition.DailyWorkRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ DailyWorkRepetition. يخلق مثيلاً جديدًا لفئة DailyWorkRepetition"
type: docs
weight: 10
url: /ar/net/aspose.tasks/dailyworkrepetition/dailyworkrepetition/
---
## DailyWorkRepetition constructor

يخلق مثيلاً جديدًا للفئة [`DailyWorkRepetition`](../).

```csharp
public DailyWorkRepetition()
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

* class [DailyWorkRepetition](../)
* namespace [Aspose.Tasks](../../dailyworkrepetition/)
* assembly [Aspose.Tasks](../../../)


