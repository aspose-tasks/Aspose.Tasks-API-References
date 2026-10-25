---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ByYearWeekDayRepetition. يهيئ نسخة جديدة من فئة ByYearWeekDayRepetition"
type: docs
weight: 10
url: /ar/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

يهيئ نسخة جديدة من الفئة [`ByYearWeekDayRepetition`](../).

```csharp
public ByYearWeekDayRepetition()
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


