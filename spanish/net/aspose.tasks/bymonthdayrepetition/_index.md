---
title: "Clase ByMonthDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.ByMonthDayRepetition class. Representa un patrón basado en la posición absoluta de un día en un mes."
type: docs
weight: 170
url: /es/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Representa un patrón que se basa en la posición absoluta de un día en un mes.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Inicializa una nueva instancia de la clase `ByMonthDayRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Obtiene o establece una posición de un día en un mes en la que la tarea debe repetirse. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Obtiene o establece un número de mes que representa el intervalo en meses entre ocurrencias. |

## Ejemplos

Muestra cómo trabajar con repeticiones de día del mes al crear nuevas tareas recurrentes.

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


