---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo RecurringTaskParameters. Imposta un calendario per l'attività ricorrente. Il calendario è selezionato dalla raccolta di calendari del progetto"
type: docs
weight: 60
url: /it/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Imposta un calendario per l'attività ricorrente. Il calendario è selezionato dalla raccolta di calendari del progetto.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| progetto | Project | Il progetto con la raccolta di calendari. |
| calendarName | Stringa | Il nome del calendario. |

## Esempi

Mostra come creare un task ricorrente.

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

### Vedi anche

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


