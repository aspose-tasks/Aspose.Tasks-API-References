---
title: "ByMonthWeekDayRepetition.WeekDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ByMonthWeekDayRepetition. تحصل أو تعين نوع يوم الأسبوع الذي يجب أن تتكرر فيه المهمة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

يحصل أو يعيّن نوع يوم الأسبوع الذي يجب أن تتكرر فيه المهمة.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## الأمثلة

يوضح كيفية العمل مع تكرارات أيام الأسبوع الشهرية أثناء إنشاء مهام متكررة جديدة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


