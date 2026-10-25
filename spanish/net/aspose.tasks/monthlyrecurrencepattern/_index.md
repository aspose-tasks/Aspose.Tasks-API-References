---
title: "Clase MonthlyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.MonthlyRecurrencePattern. Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente mensual en un proyecto"
type: docs
weight: 1080
url: /es/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente mensual en un proyecto.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Inicializa una nueva instancia de la clase `MonthlyRecurrencePattern`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtiene o establece el rango de recurrencia. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Obtiene o establece el patrón de repetición recurrente. |

## Ejemplos

Muestra cómo trabajar con repeticiones de patrones de recurrencia mensual al crear tareas recurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


