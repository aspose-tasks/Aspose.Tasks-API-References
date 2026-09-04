---
title: "RecurringTaskParameters"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente dans un projet."
type: docs
weight: 245
url: /fr/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Représente l'ensemble des paramètres utilisés pour créer une tâche récurrente dans un projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Initialise une nouvelle instance de la classe [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDuration()](#getDuration--) | Obtient la durée d'une occurrence de la tâche récurrente. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Obtient une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsque des ressources sont disponibles pour travailler dessus. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Obtient le modèle de récurrence de la tâche récurrente. |
| [getTaskName()](#getTaskName--) | Obtient le nom de la tâche récurrente. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Définissez un calendrier pour la tâche récurrente. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Définit la durée d'une occurrence de la tâche récurrente. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Définit une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsque des ressources sont disponibles pour travailler dessus. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Définit le modèle de récurrence de la tâche récurrente. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Définit le nom de la tâche récurrente. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Initialise une nouvelle instance de la classe [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtient la durée d'une occurrence de la tâche récurrente.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Obtient une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsque des ressources sont disponibles pour travailler dessus.

**Returns:**
boolean - une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsqu'aucune ressource n'est disponible pour travailler dessus.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Obtient le modèle de récurrence de la tâche récurrente.

--------------------

Peut être l'une des valeurs de l'énumération `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Obtient le nom de la tâche récurrente.

**Returns:**
java.lang.String - le nom de la tâche récurrente.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Définir un calendrier pour la tâche récurrente. Le calendrier est sélectionné dans la collection de calendriers du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Le projet avec la collection de calendriers. |
| calendarName | java.lang.String | Le nom du calendrier. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Définit la durée d'une occurrence de la tâche récurrente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | L'instance de la classe `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)). |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Définit une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsque des ressources sont disponibles pour travailler dessus.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut planifier la tâche récurrente même si elle ne se produit pas lorsqu'aucune ressource n'est disponible pour travailler dessus. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Définit le modèle de récurrence de la tâche récurrente.

--------------------

Peut être l'une des valeurs de l'énumération `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | le modèle de récurrence de la tâche récurrente. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Définit le nom de la tâche récurrente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le nom de la tâche récurrente. |

