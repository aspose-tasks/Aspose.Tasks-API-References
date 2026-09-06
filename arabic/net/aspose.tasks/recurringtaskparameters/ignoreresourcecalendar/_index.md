---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية RecurringTaskParameters. تحصل أو تعيين قيمة تشير إلى ما إذا كان سيتم جدولة المهمة المتكررة حتى إذا لم يحدث ذلك عندما تكون أي موارد متاحة للعمل عليها"
type: docs
weight: 30
url: /ar/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب جدولة المهمة المتكررة حتى إذا لم يحدث ذلك عندما تكون أي موارد متاحة للعمل عليها.

```csharp
public bool IgnoreResourceCalendar { get; set; }
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


