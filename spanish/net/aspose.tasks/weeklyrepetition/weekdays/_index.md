---
title: "WeeklyRepetition.WeekDays"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad WeeklyRepetition. Obtiene o establece un tipo de días de la semana"
type: docs
weight: 20
url: /es/net/aspose.tasks/weeklyrepetition/weekdays/
---
## WeeklyRepetition.WeekDays property

Obtiene o establece un tipo de días de la semana.

```csharp
public WeekdayType WeekDays { get; set; }
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

* enum [WeekdayType](../../weekdaytype/)
* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


