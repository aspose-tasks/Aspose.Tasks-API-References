---
title: "ByYearWeekDayRepetition.Month"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ByYearWeekDayRepetition. Obtiene o establece un mes en el que la tarea debe repetirse"
type: docs
weight: 20
url: /es/net/aspose.tasks/byyearweekdayrepetition/month/
---
## ByYearWeekDayRepetition.Month property

Obtiene o establece un mes en el que la tarea debe repetirse.

```csharp
public Month Month { get; set; }
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

* enum [Month](../../month/)
* class [ByYearWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../byyearweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


