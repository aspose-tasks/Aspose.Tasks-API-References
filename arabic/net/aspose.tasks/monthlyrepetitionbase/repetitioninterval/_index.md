---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MonthlyRepetitionBase. تُحصل أو تُعيّن عدد الأشهر الذي يمثل الفاصل بالأشهر بين التكرارات"
type: docs
weight: 10
url: /ar/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

يحصل أو يضبط عدد الأشهر الذي يمثل الفاصل الزمني بين التكرارات.

```csharp
public int RepetitionInterval { get; set; }
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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


