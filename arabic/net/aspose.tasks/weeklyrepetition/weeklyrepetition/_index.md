---
title: "WeeklyRepetition.WeeklyRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ WeeklyRepetition. يُنشئ مثيلاً جديدًا للفئة WeeklyRepetition."
type: docs
weight: 10
url: /ar/net/aspose.tasks/weeklyrepetition/weeklyrepetition/
---
## WeeklyRepetition constructor

يُنشئ مثيلاً جديدًا للفئة [`WeeklyRepetition`](../).

```csharp
public WeeklyRepetition()
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

* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


