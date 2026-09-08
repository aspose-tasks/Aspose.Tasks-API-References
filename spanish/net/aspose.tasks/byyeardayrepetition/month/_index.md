---
title: "ByYearDayRepetition.Month"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ByYearDayRepetition. Obtiene o establece un mes en el que la tarea debe ser recurrente"
type: docs
weight: 30
url: /es/net/aspose.tasks/byyeardayrepetition/month/
---
## ByYearDayRepetition.Month property

Obtiene o establece un mes en el que la tarea debe repetirse.

```csharp
public Month Month { get; set; }
```

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

* enum [Month](../../month/)
* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


