---
title: "RecurringTaskInfo"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les détails d'une tâche récurrente dans un projet."
type: docs
weight: 244
url: /fr/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Représente les détails d'une tâche récurrente dans un projet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Obtient un nombre de répétitions pour le modèle de récurrence quotidien. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Obtient une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien. |
| [getDuration()](#getDuration--) | Obtient la durée d'une occurrence de la tâche récurrente. |
| [getEndDate()](#getEndDate--) | Obtient la date à laquelle les occurrences se terminent. |
| [getMonthlyDay()](#getMonthlyDay--) | Obtient un nombre de jours du modèle de récurrence mensuel. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Obtient un jour du modèle de récurrence mensuel lors de l'utilisation d'un jour ordinal. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Obtient un nombre ordinal du modèle de récurrence mensuel. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Obtient un nombre de répétitions pour le modèle de récurrence mensuel lors de l'utilisation d'un jour ordinal. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Obtient un nombre de répétitions pour le modèle de récurrence mensuel. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Obtient une valeur indiquant s'il faut utiliser un jour ordinal pour le modèle de récurrence mensuel. |
| [getOccurrences()](#getOccurrences--) | Obtient un nombre d'occurrences de la tâche récurrente. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Obtient un modèle de récurrence de la tâche récurrente. |
| [getStartDate()](#getStartDate--) | Obtient la date à laquelle les occurrences commencent. |
| [getTask()](#getTask--) | Obtient la tâche parente de cette instance de la classe [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo). |
| [getUseEndDate()](#getUseEndDate--) | Obtient une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente. |
| [getWeeklyDays()](#getWeeklyDays--) | Obtient une collection de jours utilisés dans le modèle de récurrence hebdomadaire. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Obtient un nombre de répétitions pour le modèle de récurrence hebdomadaire. |
| [getYearlyDate()](#getYearlyDate--) | Obtient une date pour le modèle de récurrence annuel. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Obtient un jour de la semaine du modèle de récurrence annuel lors de l'utilisation du jour ordinal. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Obtient un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Obtient un nombre ordinal du modèle de récurrence annuel. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Obtient une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Définit un nombre de répétitions pour le modèle de récurrence quotidien. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Définit une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Définit la durée d'une occurrence de la tâche récurrente. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Définit la date de fin des occurrences. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Définit un nombre de jour du modèle de récurrence mensuel. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Définit un jour du modèle de récurrence mensuel lors de l'utilisation du jour ordinal. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Définit un nombre ordinal du modèle de récurrence mensuel. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Définit un nombre de répétitions pour le modèle de récurrence mensuel lors de l'utilisation du jour ordinal. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Définit un nombre de répétitions pour le modèle de récurrence mensuel. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence mensuel. |
| [setOccurrences(int value)](#setOccurrences-int-) | Définit un nombre d'occurrences de la tâche récurrente. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Définit un modèle de récurrence de la tâche récurrente. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Définit la date de début des occurrences. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Définit une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Définit une collection de jours utilisée dans le modèle de récurrence hebdomadaire. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Définit un nombre de répétitions pour le modèle de récurrence hebdomadaire. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Définit une date pour le modèle de récurrence annuel. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Définit un jour de la semaine du modèle de récurrence annuel lors de l'utilisation du jour ordinal. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Définit un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Définit un nombre ordinal du modèle de récurrence annuel. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Obtient un nombre de répétitions pour le modèle de récurrence quotidien.

**Returns:**
int - un nombre de répétitions pour le modèle de récurrence quotidien.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Obtient une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien.

**Returns:**
boolean - une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtient la durée d'une occurrence de la tâche récurrente.

--------------------

l'instance de la classe `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Obtient la date à laquelle les occurrences se terminent.

**Returns:**
java.util.Date - la date de fin des occurrences.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Obtient un nombre de jours du modèle de récurrence mensuel.

**Returns:**
int - un nombre de jours du modèle de récurrence mensuel.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Obtient un jour du modèle de récurrence mensuel lors de l'utilisation d'un jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un jour du modèle de récurrence mensuel lors de l'utilisation du jour ordinal.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Obtient un nombre ordinal du modèle de récurrence mensuel.

--------------------

Peut être l'une des valeurs de l'énumération [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un nombre ordinal du modèle de récurrence mensuel.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Obtient un nombre de répétitions pour le modèle de récurrence mensuel lors de l'utilisation d'un jour ordinal.

**Returns:**
int - un nombre de répétitions pour le modèle de récurrence mensuel lors de l'utilisation du jour ordinal.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Obtient un nombre de répétitions pour le modèle de récurrence mensuel.

**Returns:**
int - un nombre de répétitions pour le modèle de récurrence mensuel.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Obtient une valeur indiquant s'il faut utiliser un jour ordinal pour le modèle de récurrence mensuel.

**Returns:**
boolean - une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence mensuel.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Obtient un nombre d'occurrences de la tâche récurrente.

**Returns:**
int - un nombre d'occurrences de la tâche récurrente.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Obtient un modèle de récurrence de la tâche récurrente.

--------------------

Peut être l'une des valeurs de l'énumération `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - un modèle de récurrence de la tâche récurrente.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtient la date à laquelle les occurrences commencent.

**Returns:**
java.util.Date - la date de début des occurrences.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtient la tâche parente de cette instance de la classe [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo).

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Obtient une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente.

**Returns:**
boolean - une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Obtient une collection de jours utilisés dans le modèle de récurrence hebdomadaire.

--------------------

**Returns:**
int - une collection de jours utilisée dans le modèle de récurrence hebdomadaire.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Obtient un nombre de répétitions pour le modèle de récurrence hebdomadaire.

**Returns:**
int - un nombre de répétitions pour le modèle de récurrence hebdomadaire.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Obtient une date pour le modèle de récurrence annuel.

**Returns:**
java.util.Date - une date pour le modèle de récurrence annuel.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Obtient un jour de la semaine du modèle de récurrence annuel lors de l'utilisation du jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - un jour de la semaine du modèle de récurrence annuel lors de l'utilisation du jour ordinal.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Obtient un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [Month](../../com.aspose.tasks/month).

**Returns:**
int - un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Obtient un nombre ordinal du modèle de récurrence annuel.

--------------------

Peut être l'une des valeurs de l'énumération [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - un nombre ordinal du modèle de récurrence annuel.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Obtient une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel.

**Returns:**
boolean - une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Définit un nombre de répétitions pour le modèle de récurrence quotidien.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de répétitions pour le modèle de récurrence quotidien. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Définit une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut utiliser les jours ouvrés pour le modèle de récurrence quotidien. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Définit la durée d'une occurrence de la tâche récurrente.

--------------------

l'instance de la classe `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durée d'une occurrence de la tâche récurrente. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Définit la date de fin des occurrences.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de fin des occurrences. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Définit un nombre de jour du modèle de récurrence mensuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de jours du modèle de récurrence mensuel. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Définit un jour du modèle de récurrence mensuel lors de l'utilisation du jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un jour du modèle de récurrence mensuel lorsqu'on utilise le jour ordinal. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Définit un nombre ordinal du modèle de récurrence mensuel.

--------------------

Peut être l'une des valeurs de l'énumération [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre ordinal du modèle de récurrence mensuel. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Définit un nombre de répétitions pour le modèle de récurrence mensuel lors de l'utilisation du jour ordinal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de répétitions pour le modèle de récurrence mensuel lorsqu'on utilise le jour ordinal. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Définit un nombre de répétitions pour le modèle de récurrence mensuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de répétitions pour le modèle de récurrence mensuel. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence mensuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence mensuel. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Définit un nombre d'occurrences de la tâche récurrente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre d'occurrences de la tâche récurrente. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Définit un modèle de récurrence de la tâche récurrente.

--------------------

Peut être l'une des valeurs de l'énumération `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un modèle de récurrence de la tâche récurrente. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Définit la date de début des occurrences.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date de début des occurrences. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Définit une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut utiliser la date de fin ou un nombre d'occurrences pour la tâche récurrente. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Définit une collection de jours utilisée dans le modèle de récurrence hebdomadaire.

--------------------

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une collection de jours utilisée dans le modèle de récurrence hebdomadaire. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Définit un nombre de répétitions pour le modèle de récurrence hebdomadaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de répétitions pour le modèle de récurrence hebdomadaire. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Définit une date pour le modèle de récurrence annuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une date pour le modèle de récurrence annuel. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Définit un jour de la semaine du modèle de récurrence annuel lors de l'utilisation du jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un jour de la semaine du modèle de récurrence annuel lorsqu'on utilise le jour ordinal. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Définit un mois du modèle de récurrence annuel lors de l'utilisation du jour ordinal.

--------------------

Peut être l'une des valeurs de l'énumération [Month](../../com.aspose.tasks/month).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un mois du modèle de récurrence annuel lorsqu'on utilise le jour ordinal. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Définit un nombre ordinal du modèle de récurrence annuel.

--------------------

Peut être l'une des valeurs de l'énumération [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre ordinal du modèle de récurrence annuel. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Définit une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut utiliser le jour ordinal pour le modèle de récurrence annuel. |

