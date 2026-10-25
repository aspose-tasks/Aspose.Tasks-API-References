---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt de set parameters voor die worden gebruikt om een terugkerende taak in een project te maken."
type: docs
weight: 245
url: /nl/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Stelt de set parameters voor die worden gebruikt om een terugkerende taak in een project te maken.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Initialiseert een nieuw exemplaar van de [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDuration()](#getDuration--) | Haalt de duur op voor één optreden van de terugkerende taak. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Haalt een waarde op die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er middelen beschikbaar zijn om eraan te werken. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Haalt het terugkeerpatroon van de terugkerende taak op. |
| [getTaskName()](#getTaskName--) | Haalt de naam van de terugkerende taak op. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Stel een agenda in voor de terugkerende taak. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Stelt de duur in voor één gebeurtenis van de terugkerende taak. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Stelt een waarde in die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er middelen beschikbaar zijn om eraan te werken. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Stelt het terugkeerpatroon van de terugkerende taak in. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Stelt de naam van de terugkerende taak in. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Initialiseert een nieuw exemplaar van de [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters) klasse.

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Haalt de duur op voor één optreden van de terugkerende taak.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Haalt een waarde op die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er middelen beschikbaar zijn om eraan te werken.

**Returns:**
boolean - een waarde die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er geen middelen beschikbaar zijn om eraan te werken.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Haalt het terugkeerpatroon van de terugkerende taak op.

--------------------

Kan een van de waarden van `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeratie zijn.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Haalt de naam van de terugkerende taak op.

**Returns:**
java.lang.String - de naam van de terugkerende taak.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Stel een kalender in voor de terugkerende taak. De kalender wordt geselecteerd uit de projectkalendercollectie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Het project met kalendercollectie. |
| calendarName | java.lang.String | De naam van de kalender. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Stelt de duur in voor één gebeurtenis van de terugkerende taak.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | De instantie van `Duration`([getDuration()](../../com.aspose/tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskparameters\#setDuration-Duration-)) klasse. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Stelt een waarde in die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er middelen beschikbaar zijn om eraan te werken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er geen middelen beschikbaar zijn om eraan te werken. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Stelt het terugkeerpatroon van de terugkerende taak in.

--------------------

Kan een van de waarden van `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)) enumeratie zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | het herhalingspatroon van de terugkerende taak. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Stelt de naam van de terugkerende taak in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de naam van de terugkerende taak. |

