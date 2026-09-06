---
title: "ByYearWeekDayRepetition.WeekDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ByYearWeekDayRepetition. تحصل أو تعين نوع يوم الأسبوع الذي يجب أن تتكرر فيه المهمة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/byyearweekdayrepetition/weekday/
---
## ByYearWeekDayRepetition.WeekDay property

يحصل أو يعيّن نوع يوم الأسبوع الذي يجب أن يتكرر فيه المهمة.

```csharp
public DayOfWeek WeekDay { get; set; }
```

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

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


