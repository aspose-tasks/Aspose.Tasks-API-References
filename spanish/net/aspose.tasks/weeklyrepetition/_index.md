---
title: "Clase WeeklyRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.WeeklyRepetition. Representa un patrón basado en los días de la semana"
type: docs
weight: 3590
url: /es/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Representa un patrón basado en días de la semana.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Inicializa una nueva instancia de la clase `WeeklyRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Obtiene o establece un número de semanas que representa el intervalo en semanas entre ocurrencias. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Obtiene o establece un tipo de días de la semana. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


