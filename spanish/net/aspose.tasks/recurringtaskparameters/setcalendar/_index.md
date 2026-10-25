---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método RecurringTaskParameters. Establece un calendario para la tarea recurrente. El calendario se selecciona de la colección de calendarios del proyecto"
type: docs
weight: 60
url: /es/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Establece un calendario para la tarea recurrente. El calendario se selecciona de la colección de calendarios del proyecto.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | El proyecto con la colección de calendarios. |
| calendarName | Cadena | El nombre del calendario. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


