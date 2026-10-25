---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByYearWeekDayRepetition‑constructor. Initialiseert een nieuw exemplaar van de ByYearWeekDayRepetition‑klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

Initialiseert een nieuw exemplaar van de [`ByYearWeekDayRepetition`](../)‑klasse.

```csharp
public ByYearWeekDayRepetition()
```

## Voorbeelden

Toont hoe te werken met herhalingen van weekdagen per jaar bij het maken van nieuwe terugkerende taken.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


