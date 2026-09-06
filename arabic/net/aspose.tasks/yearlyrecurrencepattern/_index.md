---
title: "الفئة YearlyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.YearlyRecurrencePattern الفئة. يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة سنوية في مشروع"
type: docs
weight: 3690
url: /ar/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

يمثل مجموعة المعلمات المستخدمة لإنشاء مهمة متكررة سنويًا في مشروع.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | يُهيئ مثلاً جديداً من الفئة `YearlyRecurrencePattern`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | يحصل أو يحدد نطاق التكرار. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | يحصل أو يعيّن نمط موضع التكرار. |

## الأمثلة

يعرض كيفية العمل مع أنماط التكرار السنوية أثناء إنشاء مهام متكررة.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


