---
title: "ByYearWeekDayRepetition.ByYearWeekDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ByYearWeekDayRepetition. Inicializa una nueva instancia de la clase ByYearWeekDayRepetition"
type: docs
weight: 10
url: /es/net/aspose.tasks/byyearweekdayrepetition/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition constructor

Inicializa una nueva instancia de la clase [`ByYearWeekDayRepetition`](../).

```csharp
public ByYearWeekDayRepetition()
```

## Ejemplos

Muestra cómo trabajar con repeticiones de días de la semana del año al crear nuevas tareas recurrentes.

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

### Ver también

* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


