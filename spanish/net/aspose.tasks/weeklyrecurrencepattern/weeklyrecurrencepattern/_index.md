---
title: "WeeklyRecurrencePattern.WeeklyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor WeeklyRecurrencePattern. Inicializa una nueva instancia de la clase WeeklyRecurrencePattern"
type: docs
weight: 10
url: /es/net/aspose.tasks/weeklyrecurrencepattern/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern constructor

Inicializa una nueva instancia de la clase [`WeeklyRecurrencePattern`](../).

```csharp
public WeeklyRecurrencePattern()
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

* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


