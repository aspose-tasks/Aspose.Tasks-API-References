---
title: "MonthlyRecurrencePattern.MonthlyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ MonthlyRecurrencePattern. يُهيئ نسخة جديدة من فئة MonthlyRecurrencePattern"
type: docs
weight: 10
url: /ar/net/aspose.tasks/monthlyrecurrencepattern/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern constructor

يُهيئ نسخة جديدة من فئة [`MonthlyRecurrencePattern`](../).

```csharp
public MonthlyRecurrencePattern()
```

## الأمثلة

يوضح كيفية العمل مع تكرارات نمط التكرار الشهري أثناء إنشاء مهام متكررة.

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

* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


