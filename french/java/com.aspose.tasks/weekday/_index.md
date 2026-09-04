---
title: "WeekDay"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un jour de la semaine qui définit soit des jours réguliers d'une semaine, soit des jours d'exception dans un calendrier."
type: docs
weight: 352
url: /fr/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Représente un jour de la semaine qui définit soit des jours réguliers d'une semaine, soit des jours d'exception dans un calendrier.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié et la liste des périodes de travail. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié et les périodes de travail. |
| [WeekDay()](#WeekDay--) | Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Convertit le [DayOfWeek](../../com.aspose.tasks/dayofweek) de .Net en `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Crée une journée de travail par défaut. |
| [deepClone()](#deepClone--) | Renvoie une copie profonde du jour de la semaine. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getDayType()](#getDayType--) | Obtient le type d'un jour. |
| [getDayWorking()](#getDayWorking--) | Obtient une valeur indiquant si la date ou le type de jour spécifié est ouvrable. |
| [getFromDate()](#getFromDate--) | Obtient le début d'une période d'exception. |
| [getToDate()](#getToDate--) | Obtient la fin d'une période d'exception. |
| [getWorkingTime()](#getWorkingTime--) | Renvoie le temps de travail pour un jour de la semaine. |
| [getWorkingTimes()](#getWorkingTimes--) | Obtient WorkingTimeCollection pour cette instance de WeekDay. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Définit une valeur indiquant si la date ou le type de jour spécifié est ouvrable. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Définit les périodes de temps par défaut pour le jour de la semaine spécifié. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Définit le début d'une période d'exception. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Définit la fin d'une période d'exception. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dayType | int | Le type de jour spécifié. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié et la liste des périodes de travail.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dayType | int | Le type de jour spécifié. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Liste des périodes de temps de travail. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday) avec le type de jour spécifié et les périodes de travail.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dayType | int | Le type de jour spécifié. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Tableau des périodes de temps de travail. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Initialise une nouvelle instance de la classe [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Convertit le [DayOfWeek](../../com.aspose.tasks/dayofweek) de .Net en `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dw | int | Le jour de la semaine à convertir. |

**Returns:**
int - Un type de jour converti.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Crée une journée de travail par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dayType | int | Le type de jour à partir duquel créer la journée de travail par défaut. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Renvoie une copie profonde du jour de la semaine.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet à comparer avec cette instance. |

**Returns:**
booléen - **True** si l'objet spécifié est un WeekDay qui possède les mêmes valeurs FromDate, ToDate et WorkingTimes que cette instance ; sinon, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Obtient le type d'un jour.

**Returns:**
int - le type d'un jour.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Obtient une valeur indiquant si la date ou le type de jour spécifié est ouvrable.

**Returns:**
booléen - une valeur indiquant si la date ou le type de jour spécifié est ouvré.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Obtient le début d'une période d'exception.

**Returns:**
java.util.Date - le début d'une période d'exception.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Obtient la fin d'une période d'exception.

**Returns:**
java.util.Date - la fin d'une période d'exception.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Renvoie le temps de travail pour un jour de la semaine.

**Returns:**
double - Temps de travail.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Obtient WorkingTimeCollection pour cette instance WeekDay. La collection des temps de travail qui définissent le temps travaillé pendant le jour de la semaine.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Définit une valeur indiquant si la date ou le type de jour spécifié est ouvrable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la date ou le type de jour spécifié est ouvré. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Définit les périodes de temps par défaut pour le jour de la semaine spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Le jour de la semaine sur lequel définir le jour ouvré par défaut. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Définit le début d'une période d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | le début d'une période d'exception. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Définit la fin d'une période d'exception.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la fin d'une période d'exception. |

