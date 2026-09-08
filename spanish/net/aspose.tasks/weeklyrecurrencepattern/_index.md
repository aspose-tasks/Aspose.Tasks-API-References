---
title: "Clase WeeklyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.WeeklyRecurrencePattern clase. Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente semanal en un proyecto"
type: docs
weight: 3580
url: /es/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Representa el conjunto de parámetros que se usan para crear una tarea recurrente semanal en un proyecto.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Inicializa una nueva instancia de la clase `WeeklyRecurrencePattern`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtiene o establece el rango de recurrencia. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Obtiene o establece el patrón de repetición recurrente. |

## Ejemplos

Muestra cómo crear una tarea recurrente.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### Ver también

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


