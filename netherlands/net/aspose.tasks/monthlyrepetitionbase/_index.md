---
title: "Klasse MonthlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MonthlyRepetitionBase klasse. Vertegenwoordigt een basispatroon voor maandelijkse dagpositie"
type: docs
weight: 1090
url: /nl/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Stelt een basispatroon voor de maandelijkse dagpositie voor.

```csharp
public abstract class MonthlyRepetitionBase
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Haalt een aantal maanden op of stelt dit in dat het interval in maanden tussen de gebeurtenissen vertegenwoordigt. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


