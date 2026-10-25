---
title: "الفئة WeeklyRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.WeeklyRepetition. تمثل نمطًا يعتمد على أيام الأسبوع"
type: docs
weight: 3590
url: /ar/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

يمثل نمطًا يعتمد على أيام الأسبوع.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | يقوم بتهيئة نسخة جديدة من الفئة `WeeklyRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | يحصل أو يعيّن عدد الأسابيع الذي يمثل الفاصل الزمني بالأسابيع بين التكرارات. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | يحصل أو يضبط نوع أيام الأسبوع. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


