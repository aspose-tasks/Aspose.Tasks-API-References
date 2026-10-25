---
title: "الفئة ByMonthWeekDayRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ByMonthWeekDayRepetition. تمثل نمطًا يعتمد على موضع يوم الأسبوع في الشهر"
type: docs
weight: 180
url: /ar/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

يمثل نمطًا يعتمد على موضع يوم الأسبوع في شهر.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | يُهيئ نسخة جديدة من الفئة `ByMonthWeekDayRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | يحصل أو يعيّن موضع يوم الأسبوع في الشهر الذي يجب أن تتكرر فيه المهمة. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | يحصل أو يضبط عدد الأشهر الذي يمثل الفاصل الزمني بين التكرارات. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | يحصل أو يعيّن نوع يوم الأسبوع الذي يجب أن تتكرر فيه المهمة. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


