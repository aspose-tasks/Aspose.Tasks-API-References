---
title: "Clase ByMonthWeekDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ByMonthWeekDayRepetition. Representa un patrón que se basa en la posición del día de la semana en un mes"
type: docs
weight: 180
url: /es/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Representa un patrón que se basa en la posición del día de la semana en un mes.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Inicializa una nueva instancia de la clase `ByMonthWeekDayRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Obtiene o establece una posición del día de la semana en un mes en la que la tarea debe repetirse. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Obtiene o establece un número de mes que representa el intervalo en meses entre ocurrencias. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Obtiene o establece un tipo de día de la semana en el que la tarea debe repetirse. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


