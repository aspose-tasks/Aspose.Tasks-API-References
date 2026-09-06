---
title: "WeeklyRepetition.WeekDays"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WeeklyRepetition. تحصل أو تعين نوع أيام الأسبوع"
type: docs
weight: 20
url: /ar/net/aspose.tasks/weeklyrepetition/weekdays/
---
## WeeklyRepetition.WeekDays property

يحصل أو يضبط نوع أيام الأسبوع.

```csharp
public WeekdayType WeekDays { get; set; }
```

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

* enum [WeekdayType](../../weekdaytype/)
* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


