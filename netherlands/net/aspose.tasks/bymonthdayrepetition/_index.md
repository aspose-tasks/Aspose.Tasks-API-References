---
title: "Class ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ByMonthDayRepetition class. Vertegenwoordigt een patroon dat gebaseerd is op de absolute positie van een dag in een maand."
type: docs
weight: 170
url: /nl/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Stelt een patroon voor dat gebaseerd is op de absolute positie van een dag in een maand.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Initialiseert een nieuw exemplaar van de `ByMonthDayRepetition` class. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Haalt een positie van een dag in een maand op of stelt deze in waarop de taak moet terugkeren. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Haalt een aantal maanden op of stelt dit in dat het interval in maanden tussen de gebeurtenissen vertegenwoordigt. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


