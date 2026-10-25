---
title: "ByYearDayRepetition.ByYearDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ByYearDayRepetition. Inicializa una nueva instancia de la clase ByYearDayRepetition"
type: docs
weight: 10
url: /es/net/aspose.tasks/byyeardayrepetition/byyeardayrepetition/
---
## ByYearDayRepetition constructor

Inicializa una nueva instancia de la clase [`ByYearDayRepetition`](../).

```csharp
public ByYearDayRepetition()
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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


