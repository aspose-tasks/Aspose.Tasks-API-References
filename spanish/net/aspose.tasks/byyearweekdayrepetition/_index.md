---
title: "Clase ByYearWeekDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ByYearWeekDayRepetition. Representa un patrón basado en la posición de un día de la semana en un mes"
type: docs
weight: 200
url: /es/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Representa un patrón que se basa en la posición de un día de la semana en un mes.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Inicializa una nueva instancia de la clase `ByYearWeekDayRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Obtiene o establece un mes en el que la tarea debe repetirse. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Obtiene o establece una posición del día en una semana de un mes en la que la tarea debe repetirse. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Obtiene o establece un tipo de día de la semana en el que la tarea debe repetirse. |

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

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


