---
title: "RecurringTaskParameters.SetCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة RecurringTaskParameters. تعيين تقويم للمهمة المتكررة. يتم اختيار التقويم من مجموعة تقويمات المشروع"
type: docs
weight: 60
url: /ar/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

تعيين تقويم للمهمة المتكررة. يتم اختيار التقويم من مجموعة تقويمات المشروع.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المشروع | Project | المشروع مع مجموعة التقويمات. |
| calendarName | سلسلة | اسم التقويم. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


