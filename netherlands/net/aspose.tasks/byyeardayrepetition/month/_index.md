---
title: "ByYearDayRepetition.Month"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByYearDayRepetition eigenschap. Haalt of stelt een maand in waarop de taak moet terugkeren"
type: docs
weight: 30
url: /nl/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

Haalt een maand op of stelt een maand in waarop de taak moet terugkeren.

```csharp
public Month Month { get; set; }
```

## Voorbeelden

Toont hoe te werken met jaar-dag herhalingen bij het maken van nieuwe terugkerende taken.

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

### Zie ook

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


