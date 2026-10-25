---
title: "YearlyRecurrencePattern.YearlyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor YearlyRecurrencePattern. Inicializa una nueva instancia de la clase YearlyRecurrencePattern"
type: docs
weight: 10
url: /es/net/aspose.tasks/yearlyrecurrencepattern/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern constructor

Inicializa una nueva instancia de la clase [`YearlyRecurrencePattern`](../).

```csharp
public YearlyRecurrencePattern()
```

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

* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


