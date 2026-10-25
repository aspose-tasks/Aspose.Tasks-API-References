---
title: "تعداد WeekdayType."
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.WeekdayType. يمثل يوماً من أيام الأسبوع لمشروع في نسخة من الفئة RecurringTaskInfo."
type: docs
weight: 3570
url: /ar/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

يمثل يوماً من أيام الأسبوع لمشروع في نسخة من الفئة [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يشير إلى نوع يوم الأسبوع None. |
| Sunday | `1` | يشير إلى نوع يوم الأسبوع Sunday. |
| Monday | `2` | يشير إلى نوع يوم الأسبوع Monday. |
| Tuesday | `4` | يشير إلى نوع يوم الأسبوع Tuesday. |
| Wednesday | `8` | يشير إلى نوع يوم الأسبوع Wednesday. |
| Thursday | `10` | يشير إلى نوع يوم الأسبوع Thursday. |
| Friday | `20` | يشير إلى نوع يوم الأسبوع Friday. |
| Saturday | `40` | يشير إلى نوع يوم الأسبوع Saturday. |

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


