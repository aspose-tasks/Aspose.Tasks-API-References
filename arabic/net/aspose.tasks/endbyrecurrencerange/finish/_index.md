---
title: "EndByRecurrenceRange.Finish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية EndByRecurrenceRange. تحصل أو تعين التاريخ الذي يحد من نطاق التكرار للمهمة المتكررة."
type: docs
weight: 20
url: /ar/net/aspose.tasks/endbyrecurrencerange/finish/
---
## EndByRecurrenceRange.Finish property

يحصل أو يعيّن التاريخ الذي يحد نطاق التكرار للمهمة المتكررة.

```csharp
public DateTime Finish { get; set; }
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

* class [EndByRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endbyrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


