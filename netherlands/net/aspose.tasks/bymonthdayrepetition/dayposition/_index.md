---
title: "ByMonthDayRepetition.DayPosition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByMonthDayRepetition eigenschap. Haalt een positie van een dag in een maand op of stelt deze in waarop de taak moet terugkeren"
type: docs
weight: 20
url: /nl/net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

Haalt een positie van een dag in een maand op of stelt deze in waarop de taak moet terugkeren.

```csharp
public int DayPosition { get; set; }
```

## Voorbeelden

Toont hoe te werken met maand‑dag herhalingen bij het maken van nieuwe terugkerende taken.

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

### Zie ook

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


