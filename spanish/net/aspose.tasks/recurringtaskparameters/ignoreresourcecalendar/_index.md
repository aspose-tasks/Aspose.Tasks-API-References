---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad RecurringTaskParameters. Obtiene o establece un valor que indica si se programa la tarea recurrente incluso cuando no hay recursos disponibles para trabajar en ella"
type: docs
weight: 30
url: /es/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Obtiene o establece un valor que indica si programar la tarea recurrente incluso cuando no hay recursos disponibles para trabajar en ella.

```csharp
public bool IgnoreResourceCalendar { get; set; }
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


