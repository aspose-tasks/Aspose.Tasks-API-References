---
title: "ByMonthDayRepetition.DayPosition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ByMonthDayRepetition. تحصل أو تعين موضع اليوم في الشهر الذي يجب أن تتكرر فيه المهمة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

يحصل أو يضبط موضع يوم في الشهر الذي يجب أن تتكرر فيه المهمة.

```csharp
public int DayPosition { get; set; }
```

## الأمثلة

يوضح كيفية العمل مع تكرارات أيام الشهر أثناء إنشاء مهام متكررة جديدة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


