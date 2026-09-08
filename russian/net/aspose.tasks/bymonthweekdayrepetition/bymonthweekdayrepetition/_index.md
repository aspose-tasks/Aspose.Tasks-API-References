---
title: "ByMonthWeekDayRepetition.ByMonthWeekDayRepetition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ByMonthWeekDayRepetition. Инициализирует новый экземпляр класса ByMonthWeekDayRepetition"
type: docs
weight: 10
url: /ru/net/aspose.tasks/bymonthweekdayrepetition/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition constructor

Инициализирует новый экземпляр класса [`ByMonthWeekDayRepetition`](../).

```csharp
public ByMonthWeekDayRepetition()
```

## Примеры

Показывает, как работать с повторениями дней недели по месяцам при создании новых повторяющихся задач.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


