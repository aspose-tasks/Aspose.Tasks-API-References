---
title: "WeeklyRepetitionBase.RepetitionInterval"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WeeklyRepetitionBase. يحصل أو يضبط عدد الأسابيع الذي يمثل الفاصل بالأسابيع بين التكرارات"
type: docs
weight: 10
url: /ar/net/aspose.tasks/weeklyrepetitionbase/repetitioninterval/
---
## WeeklyRepetitionBase.RepetitionInterval property

يحصل أو يعيّن عدد الأسابيع الذي يمثل الفاصل الزمني بالأسابيع بين التكرارات.

```csharp
public int RepetitionInterval { get; set; }
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

* class [WeeklyRepetitionBase](../)
* namespace [Aspose.Tasks](../../weeklyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


