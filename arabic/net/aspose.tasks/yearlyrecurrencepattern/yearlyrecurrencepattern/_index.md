---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ YearlyRecurrencePattern. يهيئ مثيلاً جديداً من الفئة YearlyRecurrencePattern"
type: docs
weight: 10
url: /ar/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

يُهيئ مثيلاً جديداً من الفئة [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
```

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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


