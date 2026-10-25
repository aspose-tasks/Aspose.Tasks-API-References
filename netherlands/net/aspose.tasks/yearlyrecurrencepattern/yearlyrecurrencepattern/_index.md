---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "YearlyRecurrencePattern constructor. Initialiseert een nieuw exemplaar van de YearlyRecurrencePattern-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Initialiseert een nieuw exemplaar van de [`YearlyRecurrencePattern`](../) klasse.

```csharp
public YearlyRecurrencePattern()
```

## Voorbeelden

Toont hoe te werken met year year terugkeerpatronen bij het maken van terugkerende taken.

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

### Zie ook

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


