---
title: "WeeklyRecurrencePattern.Repetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WeeklyRecurrencePattern. تحصل أو تعين نمط التكرار المتكرر"
type: docs
weight: 20
url: /ar/net/aspose.tasks/weeklyrecurrencepattern/repetition/
---
## WeeklyRecurrencePattern.Repetition property

يحصل أو يعيّن نمط التكرار المتكرر.

```csharp
public WeeklyRepetitionBase Repetition { get; set; }
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

* class [WeeklyRepetitionBase](../../weeklyrepetitionbase/)
* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


