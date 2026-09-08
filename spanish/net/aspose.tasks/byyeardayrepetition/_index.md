---
title: "Clase ByYearDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ByYearDayRepetition. Representa un patrón basado en la posición absoluta de un día en un mes"
type: docs
weight: 190
url: /es/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Representa un patrón que se basa en la posición absoluta de un día en un mes.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Inicializa una nueva instancia de la clase `ByYearDayRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Obtiene o establece una posición del día en un mes en la que la tarea debe ser recurrente. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Obtiene o establece un mes en el que la tarea debe repetirse. |

## Ejemplos

Muestra cómo trabajar con repeticiones de día del año al crear nuevas tareas recurrentes.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


