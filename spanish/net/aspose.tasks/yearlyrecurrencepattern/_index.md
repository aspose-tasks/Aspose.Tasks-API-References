---
title: "Clase YearlyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.YearlyRecurrencePattern. Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente anual en un proyecto"
type: docs
weight: 3690
url: /es/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente anual en un proyecto.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Inicializa una nueva instancia de la clase `YearlyRecurrencePattern`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtiene o establece el rango de recurrencia. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Obtiene o establece el patrón de posición recurrente. |

## Ejemplos

Muestra cómo trabajar con patrones de recurrencia anual al crear tareas recurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


