---
title: "الفئة ByMonthDayRepetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.ByMonthDayRepetition class. يمثل نمطًا يعتمد على الموضع المطلق ليوم في الشهر"
type: docs
weight: 170
url: /ar/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

يمثل نمطًا يعتمد على الموضع المطلق ليوم في شهر.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | يُنشئ مثيلًا جديدًا للفئة `ByMonthDayRepetition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | يحصل أو يضبط موضع يوم في الشهر الذي يجب أن تتكرر فيه المهمة. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | يحصل أو يضبط عدد الأشهر الذي يمثل الفاصل الزمني بين التكرارات. |

## الأمثلة

يوضح كيفية العمل مع تكرارات أيام الشهر أثناء إنشاء مهام متكررة جديدة.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


