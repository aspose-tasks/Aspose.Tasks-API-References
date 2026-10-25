---
title: "WeeklyRepetitionBase.RepetitionInterval"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad WeeklyRepetitionBase. Obtiene o establece un número de semanas que representa el intervalo en semanas entre ocurrencias"
type: docs
weight: 10
url: /es/net/aspose.tasks/weeklyrepetitionbase/repetitioninterval/
---
## WeeklyRepetitionBase.RepetitionInterval property

Obtiene o establece un número de semanas que representa el intervalo en semanas entre ocurrencias.

```csharp
public int RepetitionInterval { get; set; }
```

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

* class [WeeklyRepetitionBase](../)
* namespace [Aspose.Tasks](../../weeklyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


