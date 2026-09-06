---
title: "الفئة ByYearDayRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ByYearDayRepetition. تمثّل نمطًا يعتمد على الموضع المطلق ليوم في شهر"
type: docs
weight: 190
url: /ar/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

يمثل نمطًا يعتمد على الموضع المطلق ليوم في شهر.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | يُهيئ مثيلًا جديدًا من الفئة `ByYearDayRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | يحصل أو يعيّن موضع اليوم في الشهر الذي يجب أن تتكرر فيه المهمة. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | يحصل أو يعيّن شهرًا يجب أن يتكرر فيه المهمة. |

## الأمثلة

يعرض كيفية العمل مع تكرارات اليوم السنوي أثناء إنشاء مهام متكررة جديدة.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


