---
title: "الفئة YearlyRepetitionBase"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.YearlyRepetitionBase. تمثل نمطًا أساسيًا لموقع اليوم السنوي"
type: docs
weight: 3700
url: /ar/net/aspose.tasks/yearlyrepetitionbase/
---
## YearlyRepetitionBase class

يمثل نمطًا أساسيًا لموضع اليوم السنوي.

```csharp
public abstract class YearlyRepetitionBase
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


