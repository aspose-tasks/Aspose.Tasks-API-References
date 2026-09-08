---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MonthlyRepetitionBase. Obtiene o establece un número de meses que representa el intervalo en meses entre ocurrencias"
type: docs
weight: 10
url: /es/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

Obtiene o establece un número de mes que representa el intervalo en meses entre ocurrencias.

```csharp
public int RepetitionInterval { get; set; }
```

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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


