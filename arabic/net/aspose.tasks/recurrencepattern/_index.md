---
title: "تعداد RecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.RecurrencePattern. يمثل نوع نمط تكرار لمهمة متكررة"
type: docs
weight: 1690
url: /ar/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

يمثل نوع نمط التكرار لمهمة متكررة.

```csharp
[Flags]
public enum RecurrencePattern
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Daily | `1` | نمط يومي. |
| Weekly | `4` | نمط أسبوعي. |
| Monthly | `8` | نمط شهري. |
| Yearly | `10` | نمط سنوي. |

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


