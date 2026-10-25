---
title: "الفئة RecurringTaskParameters"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.RecurringTaskParameters. تمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة في مشروع"
type: docs
weight: 1730
url: /ar/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة في مشروع.

```csharp
public class RecurringTaskParameters
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | ينشئ مثيلاً جديداً للفئة `RecurringTaskParameters`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | يحصل أو يعيّن المدة لحدوث واحد للمهمة المتكررة. المثيل من الفئة [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب جدولة المهمة المتكررة حتى إذا لم يحدث ذلك عندما تكون أي موارد متاحة للعمل عليها. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | يحصل أو يعيّن نمط التكرار للمهمة المتكررة. يمكن أن يكون أحد قيم تعداد [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | يحصل أو يعيّن اسم المهمة المتكررة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | تعيين تقويم للمهمة المتكررة. يتم اختيار التقويم من مجموعة تقويمات المشروع. |

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


