---
title: "الفئة WeeklyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WeeklyRecurrencePattern. تمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة أسبوعيًا في مشروع."
type: docs
weight: 3580
url: /ar/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة أسبوعيًا في مشروع.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | يُنشئ مثيلًا جديدًا للفئة `WeeklyRecurrencePattern`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | يحصل أو يحدد نطاق التكرار. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | يحصل أو يعيّن نمط التكرار المتكرر. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


