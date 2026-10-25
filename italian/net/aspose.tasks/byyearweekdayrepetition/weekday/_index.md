---
title: "ByYearWeekDayRepetition.WeekDay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ByYearWeekDayRepetition. Ottiene o imposta un tipo di giorno della settimana in cui l'attività deve ripetersi"
type: docs
weight: 40
url: /it/net/aspose.tasks/byyearweekdayrepetition/weekday/
---
## ByYearWeekDayRepetition.WeekDay property

Ottiene o imposta un tipo di giorno della settimana in cui l'attività deve essere ricorrente.

```csharp
public DayOfWeek WeekDay { get; set; }
```

## Esempi

Mostra come gestire le ripetizioni dei giorni della settimana su base annua durante la creazione di nuove attività ricorrenti.

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

### Vedi anche

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


