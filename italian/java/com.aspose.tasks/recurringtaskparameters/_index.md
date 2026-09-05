---
title: "RecurringTaskParameters"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta l'insieme dei parametri utilizzati per creare un'attività ricorrente in un progetto."
type: docs
weight: 245
url: /it/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Rappresenta l'insieme dei parametri utilizzati per creare un'attività ricorrente in un progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Inizializza una nuova istanza della classe [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDuration()](#getDuration--) | Restituisce la durata per una singola occorrenza dell'attività ricorrente. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Restituisce un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Restituisce il modello di ricorrenza dell'attività ricorrente. |
| [getTaskName()](#getTaskName--) | Restituisce il nome dell'attività ricorrente. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Imposta un calendario per l'attività ricorrente. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Imposta la durata per una singola occorrenza dell'attività ricorrente. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Imposta un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Imposta il modello di ricorrenza dell'attività ricorrente. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Imposta il nome dell'attività ricorrente. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Inizializza una nuova istanza della classe [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Restituisce la durata per una singola occorrenza dell'attività ricorrente.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Restituisce un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci.

**Returns:**
boolean - un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Restituisce il modello di ricorrenza dell'attività ricorrente.

--------------------

Può essere uno dei valori dell'enumerazione `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Restituisce il nome dell'attività ricorrente.

**Returns:**
java.lang.String - il nome dell'attività ricorrente.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Imposta un calendario per l'attività ricorrente. Il calendario è selezionato dalla raccolta di calendari del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Il progetto con la raccolta di calendari. |
| calendarName | java.lang.String | Il nome del calendario. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Imposta la durata per una singola occorrenza dell'attività ricorrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | L'istanza della classe `Duration`([getDuration()](../../com.aspose/tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/recurringtaskparameters\#setDuration-Duration-)). |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Imposta un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando sono disponibili risorse per lavorarci. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Imposta il modello di ricorrenza dell'attività ricorrente.

--------------------

Può essere uno dei valori dell'enumerazione `RecurrencePattern`([getRecurrencePattern()](../../com.aspose/tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose/tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | il modello di ricorrenza dell'attività ricorrente. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Imposta il nome dell'attività ricorrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il nome dell'attività ricorrente. |

