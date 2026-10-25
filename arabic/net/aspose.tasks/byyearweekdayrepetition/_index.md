---
title: "الفئة ByYearWeekDayRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ByYearWeekDayRepetition. تمثل نمطًا يعتمد على موضع يوم الأسبوع في الشهر."
type: docs
weight: 200
url: /ar/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

يمثل نمطًا يعتمد على موضع يوم الأسبوع في شهر.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | ينشئ نسخة جديدة من الفئة `ByYearWeekDayRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | يحصل أو يعيّن شهرًا يجب أن يتكرر فيه المهمة. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | يحصل أو يعيّن موضع اليوم في أسبوع من شهر يجب أن يتكرر فيه المهمة. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | يحصل أو يعيّن نوع يوم الأسبوع الذي يجب أن يتكرر فيه المهمة. |

## الأمثلة

يوضح كيفية العمل مع تكرارات أيام الأسبوع السنوية أثناء إنشاء مهام متكررة جديدة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


