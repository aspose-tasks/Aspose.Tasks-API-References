---
title: "YearlyRecurrencePattern.Repetition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية YearlyRecurrencePattern. يحصل أو يضبط نمط الموضع المتكرر"
type: docs
weight: 20
url: /ar/net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

يحصل أو يعيّن نمط موضع التكرار.

```csharp
public YearlyRepetitionBase Repetition { get; set; }
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

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


