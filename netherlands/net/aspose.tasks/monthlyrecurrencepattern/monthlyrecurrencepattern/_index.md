---
title: "MonthlyRecurrencePattern.MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MonthlyRecurrencePattern-constructeur. Initialiseert een nieuw exemplaar van de MonthlyRecurrencePattern-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/monthlyrecurrencepattern/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern constructor

Initialiseert een nieuw exemplaar van de [`MonthlyRecurrencePattern`](../)-klasse.

```csharp
public MonthlyRecurrencePattern()
```

## Voorbeelden

Toont hoe te werken met maandelijkse terugkeerpatroonherhalingen bij het maken van terugkerende taken.

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

* class [MonthlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../monthlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


