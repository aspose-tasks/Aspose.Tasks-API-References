---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar den uppsättning parametrar som används för att skapa en återkommande uppgift i ett projekt."
type: docs
weight: 245
url: /sv/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Representerar den uppsättning parametrar som används för att skapa en återkommande uppgift i ett projekt.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Initierar en ny instans av klassen [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDuration()](#getDuration--) | Hämtar varaktigheten för en förekomst av den återkommande uppgiften. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Hämtar ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Hämtar återkommandemönstret för den återkommande uppgiften. |
| [getTaskName()](#getTaskName--) | Hämtar namnet på den återkommande uppgiften. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Ställ in en kalender för den återkommande uppgiften. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ställer in varaktigheten för en förekomst av den återkommande uppgiften. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Ställer in ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Ställer in återkommandemönstret för den återkommande uppgiften. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Ställer in namnet på den återkommande uppgiften. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Initierar en ny instans av klassen [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Hämtar varaktigheten för en förekomst av den återkommande uppgiften.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Hämtar ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den.

**Returns:**
boolean - ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Hämtar återkommandemönstret för den återkommande uppgiften.

--------------------

Kan vara ett av värdena i `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-))-enumerationen.

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Hämtar namnet på den återkommande uppgiften.

**Returns:**
java.lang.String - namnet på den återkommande uppgiften.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Ställ in en kalender för den återkommande uppgiften. Kalendern väljs från projektets kalendersamling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projektet med kalendersamling. |
| calendarName | java.lang.String | Namnet på kalendern. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ställer in varaktigheten för en förekomst av den återkommande uppgiften.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Instansen av `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-))-klassen. |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Ställer in ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om den återkommande uppgiften ska schemaläggas även om den inte kan utföras när några resurser är tillgängliga för att arbeta med den. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Ställer in återkommandemönstret för den återkommande uppgiften.

--------------------

Kan vara ett av värdena i `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-))-enumerationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | återkommandemönstret för den återkommande uppgiften. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Ställer in namnet på den återkommande uppgiften.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | namnet på den återkommande uppgiften. |

