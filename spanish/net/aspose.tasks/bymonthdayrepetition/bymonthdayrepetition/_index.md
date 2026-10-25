---
title: "ByMonthDayRepetition.ByMonthDayRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ByMonthDayRepetition. Inicializa una nueva instancia de la clase ByMonthDayRepetition"
type: docs
weight: 10
url: /es/net/aspose.tasks/bymonthdayrepetition/bymonthdayrepetition/
---
## ByMonthDayRepetition constructor

Inicializa una nueva instancia de la clase [`ByMonthDayRepetition`](../).

```csharp
public ByMonthDayRepetition()
```

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

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


