---
title: "الفئة WeeklyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.WeeklyRepetitionBase. تمثل فئة أساسية للتكرارات في نمط التكرار الأسبوعي."
type: docs
weight: 3600
url: /ar/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

يمثل الفئة الأساسية للتكرارات في نمط التكرار الأسبوعي.

```csharp
public abstract class WeeklyRepetitionBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | يحصل أو يعيّن عدد الأسابيع الذي يمثل الفاصل الزمني بالأسابيع بين التكرارات. |

## الأمثلة

يوضح كيفية إنشاء مهمة متكررة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


