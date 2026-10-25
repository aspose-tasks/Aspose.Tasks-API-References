---
title: "الفئة EndByRecurrenceRange"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.EndByRecurrenceRange. تمثل نطاق التكرار للمهمة المتكررة التي يحدها يوم الانتهاء"
type: docs
weight: 510
url: /ar/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

يمثل نطاق التكرار للمهمة المتكررة الذي يحده يوم الانتهاء.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | ينشئ مثيلاً جديدًا للفئة `EndByRecurrenceRange`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | يحصل أو يعيّن التاريخ الذي يحد نطاق التكرار للمهمة المتكررة. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | يحصل أو يعيّن تاريخ بدء نطاق التكرار للمهمة المتكررة. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


