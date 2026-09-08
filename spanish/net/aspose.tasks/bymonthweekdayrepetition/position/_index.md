---
title: "ByMonthWeekDayRepetition.Position"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ByMonthWeekDayRepetition. Obtiene o establece una posición del día de la semana en un mes en la que la tarea debe repetirse."
type: docs
weight: 20
url: /es/net/aspose.tasks/bymonthweekdayrepetition/position/
---
## ByMonthWeekDayRepetition.Position property

Obtiene o establece una posición del día de la semana en un mes en la que la tarea debe repetirse.

```csharp
public OrdinalNumber Position { get; set; }
```

## Ejemplos

Muestra cómo trabajar con repeticiones de días de la semana del mes al crear nuevas tareas recurrentes.

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

### Ver también

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


