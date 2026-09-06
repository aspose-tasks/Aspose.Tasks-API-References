---
title: "الفئة MonthlyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.MonthlyRecurrencePattern. تمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة شهرية في مشروع."
type: docs
weight: 1080
url: /ar/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة شهرية في مشروع.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | يُهيئ نسخة جديدة من الفئة `MonthlyRecurrencePattern`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | يحصل أو يحدد نطاق التكرار. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | يحصل أو يعيّن نمط التكرار المتكرر. |

## الأمثلة

يوضح كيفية العمل مع تكرارات نمط التكرار الشهري أثناء إنشاء مهام متكررة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


