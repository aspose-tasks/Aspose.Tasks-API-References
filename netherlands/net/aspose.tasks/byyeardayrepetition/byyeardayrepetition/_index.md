---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByYearDayRepetition constructor. Initialiseert een nieuwe instantie van de ByYearDayRepetition-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

Initialiseert een nieuwe instantie van de [`ByYearDayRepetition`](../)-klasse.

```csharp
public ByYearDayRepetition()
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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


